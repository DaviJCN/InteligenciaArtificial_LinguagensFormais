# Resolução dos Exercícios Práticos para Fixação

---

## Bloco 1 (Derivação)

**Dada a gramática G₁:**
* **S → aS | b**

### A) Gere a palavra `aaab`.

**Passos da derivação:**
1. `S` ⇒ `aS` *(aplicando S → aS)*
2. `aS` ⇒ `aaS` *(aplicando S → aS)*
3. `aaS` ⇒ `aaaS` *(aplicando S → aS)*
4. `aaaS` ⇒ `aaab` *(aplicando S → b)*

**Resultado:** `S ⇒* aaab`

---

### B) Explique como você sabe que a derivação terminou.

A derivação termina quando a forma sentencial gerada é formada **apenas por símbolos terminais** (neste caso, as letras 'a' e 'b'). Não resta nenhum **símbolo não-terminal** (como o 'S') para ser expandido ou substituído por regras de produção.

---

## Bloco 2 (GLC - Gramática Livre de Contexto)

**Dada a gramática G₂:**
* **S → aSb | ε** *(onde ε representa a cadeia vazia)*

### A) Gere a palavra `aaabbb`.

**Passos da derivação:**
1. `S` ⇒ `aSb` *(aplicando S → aSb)*
2. `aSb` ⇒ `aaSbb` *(aplicando S → aSb)*
3. `aaSbb` ⇒ `aaaSbbb` *(aplicando S → aSb)*
4. `aaaSbbb` ⇒ `aaabbb` *(aplicando S → ε)*

**Resultado:** `S ⇒* aaabbb`

---

### B) É possível gerar `aabbb`? Justifique.

**Resposta:** **Não**, não é possível.

**Justificativa:**
A gramática G₂ gera a linguagem $L(G₂) = \{a^n b^n | n \ge 0\}$. Cada aplicação da regra `S → aSb` insere **simultaneamente** exatamente **um 'a' à esquerda** e **um 'b' à direita**. 

Consequentemente, qualquer palavra gerada por G₂ precisa ter **o mesmo número de letras 'a' e 'b'**. Como a palavra `aabbb` possui 2 letras 'a' e 3 letras 'b', ela não pode ser gerada por essa gramática.

---

## Bloco 3 (Classificação)

**Dada a gramática:**
* **S → aA**
* **A → b**

### Classifique como Regular ou Livre de Contexto:

**Classificação:** **Gramática Regular** *(Linar à Direita)*.

**Justificativa:**
- Uma gramática é **Regular (Linear à Direita)** se todas as suas produções seguem o formato $N 	o tN$ ou $N 	o t$ (onde $N$ é não-terminal e $t$ é terminal).
  - `S → aA` (Não-terminal gerando terminal + não-terminal)
  - `A → b` (Não-terminal gerando apenas terminal)
- *Nota:* Toda gramática regular também é por definição uma Gramática Livre de Contexto (GLC), mas a sua classificação mais específica e restrita é **Gramática Regular**.
