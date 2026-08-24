Considere:

Σ = a , b , c

Responda:

    Quantos símbolos existem no alfabeto? 3
    Quais são os símbolos? a,b, c
    O símbolo a pertence ao alfabeto? Sim
    O símbolo d pertence ao alfabeto? Não
    Escreva uma palavra formada por símbolos desse alfabeto. caba,aba,

---------------------------

Considere:

Σ = 0 , 1

Classifique cada sequência como palavra válida ou não válida:
Sequência 	Válida? 	Justificativa
0101 		Sim          Está dentro do alfabeto
00110 		Sim          Está dentro do alfabeto   
012 		Não          2 Não está dentro do alfabeto   
111 		Sim          Está dentro do alfabeto
10a 		Não          a Não está dentro do alfabeto


-----------------------------


Considere:

Σ = 0 , 1

Determine se as afirmações são verdadeiras ou falsas:

    0 ∈ Σ - Verdadeiro, 0 está no conjunto Sigma
    1 ∈ Σ - Verdadeiro, 1 está no conjunto Sigma
    01 ∈ Σ - Falso, 0 e 1 não são um simbolo inidividual
    01 ∈ Σ ∗ - Verdadeiro, Está dentro do fecho de Kleene 
    2 ∈ Σ - Falso, Não existe 2 no conjunto
    101 ∈ Σ ∗ - Verdadeiro, 101 é uma sequencia válida (fecho de Kleene)


-------------------------------

Exercício para o estudante

Considere:

L = 0 , 01 , 011 , 0111

Determine se cada palavra pertence à linguagem:

    0 ∈ L Sim
    01 ∈ L Sim
    0111 ∈ L Sim
    10 ∈ L Não
    111 ∈ L Não
    011 ∈ L Sim

---------------------------------

Considere:

L = b n ∣ n ≥ 1

    Escreva as cinco primeiras palavras. b, bb, bbb, bbbb, bbbbb
    Explique o significado de b n. n ocorrencias de b
    A palavra bbbbbb pertence à linguagem? Sim
    A palavra vazia ( ε ) pertence à linguagem? Não


----------------------------------

Exercício para o estudante

Explique, com suas próprias palavras, a diferença entre:
A

L = ∅
B

L = ε

Depois responda:

    Qual delas possui uma palavra? A
    Qual delas não possui nenhuma palavra? B
    Qual é o comprimento da palavra ε ? Zero


----------------------------------------------


G = ( S , A , 0 , 1 , P , S )

    Conjunto de variáveis**: {S, A}
    Conjunto de terminais**: {0, 1}
    Conjunto de produções**: {S → 0 A, A → 1}
    Símbolo inicial**: S
    Palavras geradas**: {01}

-------------------------------------------------
    Aplicar a regra uma vez**: S → 0 A → 0 1
    Aplicar a regra duas vezes**: S → 0 A → 0 1 → 0 0 1
    Aplicar a regra três vezes**: S → 0 A → 0 1 → 0 0 1 → 0 0 0 1
    Sequência completa de derivação**: S → 0 A → 0 1 → 0 0 1 → 0 0 0 1

------------------------------------------------

- **Geração de a a a b**: 
  S → a S → a a S → a a a S → a a a b

---------------------------------------------------
    **1**: Sim, derivação: S → 0 S → 0 1
    **01**: Sim, derivação: S → 0 S → 0 1
    **001**: Sim, derivação: S → 0 S → 0 1
    **0001**: Sim, derivação: S → 0 S → 0 1
    **101**: Não
    **1001**: Não








