# Resolução dos Exercícios Práticos para Fixação

---

## Bloco 1 (Derivação)

**Dada a gramática $G_1$:**
$$S \rightarrow aS \mid b$$

### A) Gere a palavra *aaab*.

**Passos da derivação:**
1. $S \Rightarrow aS$ *(aplicando a regra $S \rightarrow aS$)*
2. $aS \Rightarrow aaS$ *(aplicando a regra $S \rightarrow aS$)*
3. $aaS \Rightarrow aaaS$ *(aplicando a regra $S \rightarrow aS$)*
4. $aaaS \Rightarrow aaab$ *(aplicando a regra $S \rightarrow b$)*

**Resultado:** $S \Rightarrow^* aaab$

---

### B) Explique como você sabe que a derivação terminou.

A derivação termina quando a forma sentencial gerada é composta **exclusivamente por símbolos terminalis** (no caso, as letras 'a' e 'b'). Não há mais **símbolos não-terminais** (variáveis como '$S$') para serem substituídos por regras de produção.

---

## Bloco 2 (GLC - Gramática Livre de Contexto)

**Dada a gramática $G_2$:**
$$S \rightarrow aSb \mid \varepsilon$$

### A) Gere a palavra *aaabbb*.

**Passos da derivação:**
1. $S \Rightarrow aSb$ *(aplicando a regra $S \rightarrow aSb$)*
2. $aSb \Rightarrow aaSbb$ *(aplicando a regra $S \rightarrow aSb$)*
3. $aaSbb \Rightarrow aaaSbbb$ *(aplicando a regra $S \rightarrow aSb$)*
4. $aaaSbbb \Rightarrow aaa\varepsilon bbb = aaabbb$ *(aplicando a regra $S \rightarrow \varepsilon$)*

**Resultado:** $S \Rightarrow^* aaabbb$

---

### B) É possível gerar *aabbb*? Justifique.

**Resposta:** **Não**, não é possível.

**Justificativa:**
A gramática $G_2$ gera a linguagem $L(G_2) = \{a^n b^n \mid n \ge 0\}$, onde cada aplicação da regra $S \rightarrow aSb$ adiciona exatamente **um 'a' à esquerda** e **um 'b' à direita** simultaneamente. Portanto, todas as palavras geradas por $G_2$ possuem um número estritamente igual de símbolos 'a' e 'b'. 

A palavra *aabbb* possui 2 letras 'a' e 3 letras 'b' (quantidades diferentes), logo não pertence à linguagem gerada por $G_2$.

---

## Bloco 3 (Classificação)

**Dada a gramática:**
$$S \rightarrow aA \mid A \rightarrow b$$ 
*(Nota: as regras são $S \rightarrow aA$ e $A \rightarrow b$)*

### Classifique como Regular ou Livre de Contexto:

**Classificação:** **Gramática Regular** (e consequentemente também Livre de Contexto, já que toda gramática regular é livre de contexto).

**Justificativa:**
- Todas as regras de produção têm a forma permitida para uma **Gramática Regular (Linear à Direita)**:
  - $S \rightarrow aA$ (Símbolo não-terminal gerando um terminal seguido de um não-terminal)
  - $A \rightarrow b$ (Símbolo não-terminal gerando apenas um terminal)
- Como toda Gramática Regular cumpre os requisitos de uma Gramática Livre de Contexto (cujo lado esquerdo de cada regra é formado por um único não-terminal), ela pertence a ambas as categorias, sendo especificamente classificada como **Regular**.
