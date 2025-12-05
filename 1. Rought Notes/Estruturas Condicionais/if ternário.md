04-12-25

Status: #done

Tags: [[estruturas_condicionais]]

----

# Conceito Geral

O if ternário É uma forma resumida de escrever um if/else em uma única linha. Ele é composto por três partes, a primeira é o retorno caso a expressão retorne verdadeiro, a segunda é a expressão lógica e a terceira o retorno caso a condição seja falsa. Ex.:

```python
saldo = 1000
saque = int(input('Quanto você deseja sacar? R$'))
status = 'Sucesso' if saque <= saldo else 'Falha'
print(f'{status} ao realizar o saque.')

```

----

# Referências
Bootcamp DIO [Suzano - Python Developer](https://www.dio.me/bootcamp/suzano-python-developer)