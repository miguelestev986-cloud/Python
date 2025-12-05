28-11-25

State: #done 

Tags: [[funções_built-in]]

----

# Para que serve

dict() é uma função usada para *criar dicionários*, sejam eles *vazios* ou inicializados a partir de uma *coleção de pares chave-valor*.

----

# Parâmetros e Retorno

```python
class dict(**kwargs)
class dict(mapping, **kwargs)
class dict(iterable, **kwargs)
```

Se *não* dermos **argumentos** à função, ela criará um *dicionário vazio*.

Se dermos um **objeto de mapeamento**, um dicionário é criado com os *mesmo pares chave-valor do objeto*.

Se dermos um **iterável** (como uma lista de tuplas), cada *item do iterável tem que ser um iterável com exatos dois objetos*. O primeiro será a chave e o segundo o valor correspondente à chave. Se uma *chave ocorre mais de uma vez, o último valor da chave vira o valor correspondente à ela no novo dicionário*.

Se argumentos **kwargs** forem fornecidos, *seus valores são adicionados ao dicionário criado a partir do argumento posicional*. Se uma *chave* sendo adicionada *já estiver presente*, o valor do argumento de palavra-chave *substitui o valor do argumento posicional*.

Para ilustrar:

```python
>>> a = dict(one=1, two=2, three=3)
>>> b = {'one': 1, 'two': 2, 'three': 3}
>>> c = dict(zip(['one', 'two', 'three'], [1, 2, 3]))
>>> d = dict([('two', 2), ('one', 1), ('three', 3)])
>>> e = dict({'three': 3, 'one': 1, 'two': 2})
>>> f = dict({'one': 1, 'three': 3}, two=2)
>>> a == b == c == d == e == f
True
```

----
# Referências
Bootcamp DIO [Suzano - Python Developer](https://www.dio.me/bootcamp/suzano-python-developer)
[[Iteráveis]]
[[Objetos de Mapeamento]]
[[Argumentos]]
[[zip()]]