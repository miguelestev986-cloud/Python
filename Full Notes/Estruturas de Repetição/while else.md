04-12-25

Status: #done

Tags: [[estruturas_repetição]]

----

# Conceito Geral

Assim como **for/else**, podemos usar *else* para *executar um bloco de código quando a condição do laço while não for atendida*.

```python
senha = '1234'
entrada = input('Qual a senha?')
while entrada != '1234':
	print('Senha incorreta! Tente novamente.')
	entrada = input('Qual a senha?')
else:
	print('Bem vindo!')
```

----

# Referências
Bootcamp DIO [Suzano - Python Developer](https://www.dio.me/bootcamp/suzano-python-developer)
[[while]]
[[else]]
[[for else]]