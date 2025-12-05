05-12-25

Status: #todo

Tags: [[tipos_coleção]]

----

# Conceito

Tuplas são estruturas de dados muito *parecidas com as listas* :  podem *armazenar todos os tipos de objetos* Python; podemos *criar* estruturas bidimensionais (*tabelas*) *aninhando tuplas*, e acessar os dados informando os índices de linha e coluna. A principal diferença é que *tuplas são imutáveis*.

```python
matriz = (
	(1, 'a', 2),
	('b', 3 , 4),
)

matriz[0] # (1, 'a', 2)
matriz[0][-1] # 2
matriz[1][1] # 'b'
```

----

# Como criá-las

Podemos criar tuplas através da função **tuple** ou colocando *valores separados por vírgula entre parênteses ou só separadas por vírgula*.

```python
frutas = ("maçã", "uva", "manga")
números = 1, "Dois", 3.0
pais = ("Brasil",)
# Quando temos um único elemento numa tupla, precisamos por uma vírgula para indicar que é um tupla. Nesse caso, sem a vírgula, "Brasil" seria tratado apenas como uma string
```

----
# Acesso aos Dados

Tuplas são sequências, portanto podemos acessar seu dados utilizando *índices*; chamamos isso de *acesso direto*. O índice de uma tupla, assim como em uma lista, começa em 0.

```python 
frutas = ("maçã", "uva", "manga",)
frutas[0] # maçã
frutas[-1] # manga
```


Além de acessar os itens diretamente, podemos extrair um conjunto de valores de uma sequência com o *fatiamento*. Para isso basta passar o *índice inicial e/ou final para acessar o conjunto. Podemos informar quantas posições o cursor deve "pular" no acesso*.

```python
tupla = ('P', 'y', 't', 'h', 'o', 'n',)

tupla[2:] # ('t', 'h', 'o', 'n')
tupla[:2] # ('P', 'y')
# Assim como no fatiamento de strings, ele não considera o índice final.
tupla[0:3:2] # ('P', 't')
tupla[::] # Gera uma cópia da tupla
tupla[::-1] # Gera uma cópia inversa da tupla
```

----
# Referências
Bootcamp DIO [Suzano - Python Developer](https://www.dio.me/bootcamp/suzano-python-developer)
[[tuple()]]
