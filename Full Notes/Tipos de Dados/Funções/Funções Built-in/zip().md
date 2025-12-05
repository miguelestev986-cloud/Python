28-11-25

State: #done

Tags: [[funções_built-in]]

----

# Para que serve

Sua função é *devolver uma sequência de tuplas*. O nome da função está relacionado ao zíper, que *junta e encaixa duas carreiras de dentes*. Normalmente usamos zip na *criação de dicionários*.
Se as entradas têm comprimentos diferentes e você se importa com os valores finais serem correspondentes, use **itertools.zip_longest()

----

# Parâmetros

Ela recebe *duas ou mais sequências* (como strings, listas ou tuplas).

```python
dicionario = dict(zip(['Maria', 'João', 'Pedro'], ['M', 'J', 'P']))
# dicionario = {'Maria':'M', 'João':'J', 'Pedro', 'P'}
```

---- 
# Referências

[[itertools.zip_longest()]]