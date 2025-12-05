04-12-25

Status: #done

Tags: [[estruturas_condicionais]]

----

# Conceito Geral

Com if podemos criar um estrutura condicional composta por *um único desvio*. Ele *avalia uma expressão lógica* e, caso essa seja *verdadeira, executa o bloco de código*.

```python
idade = int(input('Qual sua idade'))
if idade >= 18:
	print('Você é maior de idade.')
```

Podemos usar *if's dentro de outros if's*, e chamamos isso de *if aninhado*.

```python
idade = int(input('Qual sua idade?'))
if idade >= 18:
	print('Você é maior de idade.')
else:
	if idade >= 16:
		emancipado = input('Você é emancipado? (s/n)')
		if emancipado == 's':
			print('Você tem os direitos e deveres de um maior de idade.')
		else:
			print('Você é menor de idade.')
	else:
		print('Você é menor de idade.')
```

----

# Referências
Bootcamp DIO [Suzano - Python Developer](https://www.dio.me/bootcamp/suzano-python-developer)
Curso em Vídeo Python - Mundo 1