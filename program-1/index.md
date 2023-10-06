# Básico

## aula1 - conhecendo a linguagem #
*tipos e quanto esse tipo custa na memória*: 
text => str
num => int, float, complex
seq => list, tuple, range
map => dict
colection => set, frozenset (lista sem repetições)
boolean => bool
binary => bytes, byteaaray, memoryview


*Modo interativo*


command=>  python3   = parar abrir terminal
command=>  dir()     = tras o escopo local
command=>  help()    = quais argumentos o metódo recebe


*Variaveis e constantes*
Não existem constantes.
Em constantes usar todas as letras maisculas por convenção
exemp = [
    'RG',
    'SP',
    'MG'
]

Padrão de nome em snake_case

*Conversão de tipos*

*Funções de entrada e saída*
Input  => input
Output => print


## Aula 2 - Tipos de operadores #

Operadores aritméticos           => +, -, *, /, **, //, %
OPeradores de compração          => >, <, <=, =>, ==, ===,
Operadores de atribuição         => +=, -=, //=, **=
Operadores lógicos (return bool) => and, or, not
Operados de identidade           =>
Operadores de associação         =>



# Intermediario

Listas
Tuplas -> é uma estrutura imutavél
Classe: tuple

```python
frutas= ("tio", "avó",)
pais = ("Brasil",) # atentar-se a virgula no final

letras = tuple("python")
numeros = tuple([1, 2, 3, 4])
```

```python
tuple = ("a", "m", "e", "i", "x", "a",)

tupla[2:] #("e", "i", "x", "a",)
tupla[:2] #("a", "m")
tupla[1:3] #("m", "e")
tupla[0:3:2] #("a", "e")
tupla[::] #("a", "m", "e", "i", "x", "a",)
tupla[::-1]# ("a", "x", "i", "e", "m", "a",)
```

().count
().index
().len


Conjuntos
set() elimina duplicidade

```python
set([1, 2, 3, 4, 5, 1, 5 ]) # {1, 2, 3, 4, 5}
set("abacaxi") # {"b", "a", "c", "x", "i"}

#no set nao podemos indexar numeros

a={1, 2}
b={2, 3, 4}
a.union(b) # 1 2 3 4
a.intersection(b) # 2
a.difference(b) #1
b.difference(a) # 3 4
a.symmetric_difference(b) # 1 3 4
a.issubset(b) # se contem algo ou nao, return boolean
a.isdisjoint(b) # verifica se ha diferenca, retorna boolean
a.add(22) #verifiac se ha, se nao houver add
a.clear() #limpa o objeto
a.copy() #faz um copia
a.discar(1) #descarta o valor se existir
a.pop() #tira o primeiro valor da lista
a.remove(0)  #remove o item se nao existir retorna erro
```

Dicionario => as chaves sao imutaveis, os valores mutaveis


(*args (tupla), **kwargs (dici))