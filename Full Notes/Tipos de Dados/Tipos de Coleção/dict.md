04-12-25

Status: #doing 

Tags:  [[tipos_coleção]]

----

# Conceito

Dicionários (dict) são um conjunto não-ordenado de pares chave-valor entre chaves separados por vírgula.

# Criação

Podemos criar dicionários colocando um conjunto de *pares chave : valor entre chaves separados por vírgula* ou usando a *função embutida **dict()***

```python
pessoa1 = {'nome' : 'Python', 'sobrenome' : 'da Silva'}
```

Há exemplos de uso da função dict() na nota [[dict()]]

# Acesso dos Valores

Podemos acessar dados de um dicionário *dando seu nome e seguido de colchetes a chave que queremos acessar o valor*.

```python
dados = {"nome": "Guilherme", "idade": 28, "telefone": "3333-1234"}

dados["nome"]  # "Guilherme"
dados["idade"]  # 28
dados["telefone"]  # "3333-1234"
```


# Edição dos Valores

Podemos editar valores *acessando suas chaves e atribuindo à elas novos valores*.

```python
ra_alunos = {
	'1ano': {
		'Maria Joaquina':'00011xxxxxxsp',
	},
}

ra_alunos['1ano']['Maria Joaquina'] = '00011yyyyyysp'
```

----

# Referências

[[R.Dicionários]]