05-12-25

State: #done

Tags: [[funções_built-in]]

----

# Para que serve

*Criar tuplas* ou *converter* algum **iterável** em uma tupla.

----

# Parâmetros e Retorno

A passagem de argumentos aos parâmeros é opcional. Se *não passarmos* nenhum argumento, será criada uma *lista vazia*. Mas podemos *passar iteráveis como argumento e ela criará uma tupla com os objetos do iterável*.

```python
lista = [1, 2, 3]
dic = {"A" : 1, "B" : 2, "C" : 3}
print(tuple(lista))
print(tuple(dic))
# Cria a tupla apenas com as chaves do dicionário

>>>(1, 2, 3)
>>>("A", "B", "C")
```
----

# Referências
Bootcamp DIO [Suzano - Python Developer](https://www.dio.me/bootcamp/suzano-python-developer)
[[Iteráveis]]