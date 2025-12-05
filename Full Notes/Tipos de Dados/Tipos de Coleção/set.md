04-12-25

Status: #done

Tags: [[tipos_coleção]]

----
# Conceito

Um conjunto (set) é uma *coleção não ordenada que não possui objetos repetidos*. Usamos sets principalmente para *representar conjuntos matemáticos ou eliminar itens duplicados de um iterável*

----
# Criação

Podemos criar um set simplesmente *definindo um coleção de objetos únicos e não ordenados dentro de chaves* ou com a função **set**

```Python
lista = [1,2,3,4,4,1,5]
tupla = (1,2,3,4,4,1,5,)
conjunto = {"Java", "Python", "Java"}

set(lista) # {1,2,3,4,5}
set(tupla) # {1,2,3,4,5}
print(conjunto) # {"Python", "Java"}
```
Obs.: Para criar conjuntos vazios nós usamos a função set sem nenhum argumento. Não podemos usar {} porque isso cria um dicionário vazio, não um conjunto vazio.

----
# Acesso dos Dados

Conjuntos *não suportam indexação (índice) e nem fatiamento*, uma vez que são não-ordenados. Caso queiramos acessar seus valores *é necessário converter o conjunto para lista*:

```python
numeros = {1, 2, 3, 4, 5}
numeros = list(numeros)
print(numeros[4])
```

Mas podemos *acessar os valores iterando o conjunto com for*:

```python
numeros = {1, 2, 3, 4, 5}
for numero in numeros:
	print(numero)
```

As vezes é necessário saber qual o *índice do objeto* dentro do laço for. Para isso usamos *enumerate*:

```python
numeros = {1, 2, 3, 4, 5}
for indice, numero in enumerate(numeros):
	print(f"{indice} : {numero}")

# Podemos usar enemurate com listas e tuplas também
```

----

# Referências
Bootcamp DIO [Suzano - Python Developer](https://www.dio.me/bootcamp/suzano-python-developer)
[[set()]]