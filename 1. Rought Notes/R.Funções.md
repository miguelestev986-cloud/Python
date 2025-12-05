### Fontes
Bootcamp DIO [Suzano - Python Developer](https://www.dio.me/bootcamp/suzano-python-developer)
Hashtag Programação [Args e Kwargs em Python - Aprenda de Uma Vez por Todas](https://www.youtube.com/@HashtagProgramacao)

# **Retorno

Para retornar um valor, utilizamos *return*. Toda função Python retorna *None* por padrão. Diferente de outras linguagens, Python permite que a função retorne mais de um valor.

```python
def dobro(número):
	dobro = número * 2
	return dobro

num = int(input('Digite um número: '))
print(f'O dobro de {num} é {dobro(num)}')
```

No caso da função retornar mais de um valor, ela retorna um *tupla* com os valores. Uma tupla em Python é uma sequência imutável de valores de qualquer tipo, o que significa que, uma vez criada, seus elementos não podem ser alterados, adicionados ou removidos. Ex.:

```python
def antec_suces(número):
	antecessor = número - 1
	sucessor = número + 1
	return antecessor, sucessor
	
antec_suces(2)

>>>(1,3)
```

# **Argumentos Nomeados

Além dos argumentos posicionados, as funções também podem ser chamadas usando argumentos nomeados na forma chave (keyword) = valor. Ex.:

```python
def save_user(usuário, senha):
	print(f'Usuário {usuário} salvo!')
save_user(usuário = "Joaquim", senha = 1234)
```

A vantagem de usar chave = valor na chamada na função é que, se por algum motivo a ordem dos parâmetros forem alterados, isso não gerará erro nas chamadas que estariam com a ordem dos valores erradas. Por outro lado, se o nome do parâmetro for alterado, as chamadas que usarem o nome antigo retornarão erro.

# **Args e kwargs

Podemos combinar parâmetros obrigatórios com args e kwargs. Quando esses são definidos (* args e ** kwargs), o método recebe os valores como tupla e dicionário respectivamente. * args permite que a função receba vários valores (sem keywords) e os junta em uma tupla:

```python
def calculo_imposto(valor, *porcentagens):
# Por convenção, sempre usamos *args mas "args" pode ter qualquer nome contanto que tenha *. 
	total = 0
	#Como *args faz uma tupla com os valores, é possível percorrê-los com for
	for item in porcentagens:
		total += valor * item
	return total

print(calculo_imposto(160, 0.10, 0.7))
```

O ** kwargs, como pode se observar no nome: "Keyword args" são como os args, ele aceita vários parâmetros pra função mas ele precisa que eles sejam passados na forma de chave = valor. Com os valores, ele cria um dicionário. Podemos substituir "kwargs" por qualquer outro nome (mantendo ** no início do nome), mas, assim como "args", usamos "kwargs" por convenção.

```python
def calculo_imposto_trimestral(valor, **kwargs):
	total = 0
	print(kwargs)
	if 'ir' in kwargs:
		total += valor * kwargs['ir'] 
	return total
print(calculo_imposto_trimestral(160, ir = 0.275))

>>>{'ir' : 0.275}
>>>44
```

Podemos usar args e kwargs nos parâmetros de uma mesma função porque o Python entende que os args acabaram e começaram os kwargs quando os parâmetros começar a ser definidos por chave = valor.

# **Parâmetros especiais

Por padrão, argumentos podem ser passados para uma função Python tanto por posição quanto explicitamente pelo nome. Para uma melhor legibilidade e desempenho, faz sentido restringir a maneira pelo qual argumentos possam ser passados, assim um desenvolvedor precisa apenas olhar para a definição da função para determinar se os itens são passados por posição, posição e nome, ou por nome. 
Os parâmetros antes de / são somente posicionais (não podem ser atribuídos valores por chave = valor). 
Os parâmetros entre / e * podem ser posicionais ou nomeados e os depois de * apenas nomeados.

Positional only:
```python
def função(pos1, pos2, /)
```

Keyword only:
```python
def função(*, kw1, kw2)
```

Hybrid:
```python
def função(pos1, pos2, /, pos_ou_chave, *, kw1, kw2)
```

# **Objetos de primeira classe

Em Python tudo é objeto, dessa forma funções também são objetos o que as tornam objetos de primeira classe. Com isso podemos atribuir funções a variáveis, passá-las como parâmetros para funções, usá-las como valores em estruturas de dados (listas, tuplas, dicionários, etc) e usar como valor de retorno para uma função (closures). Por exemplo:

```python
def somar(n1, n2):
	soma = n1 + n2
	return soma

def multiplicar(n1, n2):
	produto = n1 * n2
	return produto

def exibir(n1, n2, função):
	resultado = função(n1, n2)
	print(f'O resultado da operação é {resultado}')

exibir(2, 3, somar)
```

# **Escopo local e global

Python trabalha com escopo local e global, dentro do bloco da função o escopo é local. Portanto alterações ali feitas em objetos imutáveis serão perdidas quando o método terminar de ser executado. Para usar objetos globais utilizamos a palavra-chave "global", que informa ao interpretador que a variável que está sendo manipulada no escopo local é global. Essa NÃO é uma boa prática e deve ser evitada.

```python
salario = 2300

def bonus(porcentagem_bonus):
	global salario
	salario = salario * porcentagem_bonus
	return salario

salario_com_bonus = bonus(500)
print(salario_com_bonus)
```

Podemos usar .copy() se não quisermos alterar o valor original da referência. Uma observação é que inteiros não possuem .copy().