05-12-25

Status: #done

Tags: [[operadores]]

----

# Conceito

São operadores *utilizados em conjunto com os **operadores de comparação**, para montar uma expressão lógica* que retorna uma valor booleano.

----

# Operadores

1. and (e)
2. or (ou)
3. not (não)
4. () (delimita a precedência da expressão)

```python
print((100 * 4)/2 == 200 and 100 * 2 == 400)
>>> False

print((100 * 4)/2 == 200 or 100 * 2 == 400)
>>> True
#Apenas uma das expressões precisa ser verdadeira

print( not 100 * 2 == 400)
>>> True
```

----

# Referências
Bootcamp DIO [Suzano - Python Developer](https://www.dio.me/bootcamp/suzano-python-developer)
Curso em Vídeo Python - Mundo 1
[[Operadores de Comparação]]