28-11-25

State: #done

Tags: [[instruções]]

# Conceito

A instrução def no Python é uma palavra-chave utilizada para *definir uma função*. Dentro dos parêntese *indicamos os valores que a função irá usar (parâmetros) e o que ela fará com esses valores*, mas parâmetros não são obrigatórios. Quando chamarmos a função, passamos para a ela os ***argumentos** que atenderão aos parâmetros*. A estrutura é essa:

```python
def nome_da_função(parâmetros):
	corpo da função
```

Por exemplo, uma função que dá boas vindas à um nome:

```python
def welcome(name)
	print(f'Bem vindo {name}!')
welcome('Python')

# Nome do parâmetro é name e o argumento passado à ele na chamada da função é 'Python'
```

# Referências
Bootcamp DIO [Suzano - Python Developer](https://www.dio.me/bootcamp/suzano-python-developer)
