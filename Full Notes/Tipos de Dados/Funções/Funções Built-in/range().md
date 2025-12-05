04-12-25

State: #done

Tags: [[funções_built-in]]

----

# Para que serve

Essa função *produz uma sequência de números inteiros*.

----

# Parâmetros

Ela pode tem três parâmetros: start (opcional, por padrão ele começa em 0), stop (obrigatório) e step (opcional).

```python
print(list(range(2, 11, 3)))

# Começa em 2, vai até 11 e pula de 3 em 3
```

----

# Retorno

Essa função calcula os números sob demanda, ele não os guarda. Para retornar uma lista com a sequência dos números, precisamos usar **list()**

```python
print(list(range(2, 11, 3)))

>>>[2, 5, 8]
```

# Referências

[[list]]