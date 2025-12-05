04-12-25

Status: #done

Tags: [[estruturas_condicionais]]

----

# Conceito Geral

A condição elif permite *testar mais de uma condição além da do if* (ter mais de dois desvios), usamos elif. É uma junção de else com if, podemos usar quantos quisermos.

```python
idade = int(input('Qual sua idade'))
if idade >= 18:
	print('Você é maior de idade.')
elif idade <= 5:
	print('Você já sabe ler?!')
else:
	print('Você ainda é menor de idade.')
```

----

# Referências
Bootcamp DIO [Suzano - Python Developer](https://www.dio.me/bootcamp/suzano-python-developer)
Curso em Vídeo Python - Mundo 1