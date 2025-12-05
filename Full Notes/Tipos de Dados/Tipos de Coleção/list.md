05-12-25

Status: #todo 

Tags:

----

# Conceito

----

# Referências
Bootcamp DIO [Suzano - Python Developer](https://www.dio.me/bootcamp/suzano-python-developer)
# **O que são

Listas em Python podem armazenar de maneira sequencial qualquer tipo de objeto. Listas são objetos mutáveis, portanto podemos alterar seus valores após a criação.

# **Como criá-las

Podemos criar listas utilizando o construtor *list* , a função range ou colocando valores separados por vírgula dentro de colchetes.  Não precisamos atribuir valores a uma lista assim que a declaramos.

```python
frutas = []
letras = list('Python')
#letras = ['P', 'y', 't', 'h', 'o', 'n']
numeros = list(range(10))
#numeros = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
nomes = ['Maria', 'João', 'Pedro']
```

# **Como acessá-las

Listas são sequências, portanto podemos acessar seu dados utilizando *índices*; chamamos isso de *acesso direto*. O índice de uma lista começa em 0.

```python
letras = list('Python')
letras[0] #P
letras[1] #y
```

Podemos indicar índices negativos para acessar a lista do fim pro início :

```python
letras = list('Python')
letras[-1] #n
#Observe que o indice negativo começa em -1 e não 0
letras[-4] #t
```

Além de acessar os itens diretamente, podemos extrair um conjunto de valores de uma sequência com o *fatiamento*. Para isso basta passar o índice inicial e/ou final para acessar o conjunto. Podemos informar quantas posições o cursor deve "pular" no acesso.

```python
lista = ['P', 'y', 't', 'h', 'o', 'n']

lista[2:] # ['t', 'h', 'o', 'n']
lista[:2] #['P', 'y']
# Assim como no fatiamento de strings, ele não considera o índice final.
lista[0:3:2] # ['P', 't']
lista[::] # Gera uma cópia da lista
lista[::-1] # Gera uma cópia inversa da lista
```

Também podemos *iterar* (percorrer) os índices de uma lista com for:

```python
frutas = ['maçã', 'banana', 'uva']
for item in frutas:
	print(item)
```

# **Listas aninhadas

Listas podem armazenar todos os tipos de objetos Python, portanto podemos criar estruturas bidimensionais (tabelas), e acessar informando os índices de linha e coluna.

```python
matriz = [
	[1, 'a', 2],
	['b', 3 , 4],
]

matriz[0] # [1, 'a', 2]
matriz[0][-1] # 2
matriz[1][1] # 'b'
```

# **Compreensão de listas

A compreensão de lista oferece uma sintaxe mais curta quando você deseja criar uma lista com base nos valores de uma lista existente ou gerar uma lista aplicando alguma modificação nos elementos de uma lista existente.

Normalmente, faríamos:
```python
numeros = [1,2,3,4,5,6,7,8,9,10]
pares = []

for numero in numeros:
	if numero % 2 == 0:
		pares.append(numero)
```

Mas com compreensão, o código fica mais limpo:

```python
numeros = [1,2,3,4,5,6,7,8,9,10]
pares = [numero for numero in numeros if numero % 2 == 0]
```

A primeira parte é o retorno (o que vai compor a lista), a segunda parte é a iteração (for).  A terceira parte, que é opcional, normalmente usamos um condicional. 
"Se há um número em 'numeros' e se o resto da divisão desse número por dois for zero, adicione o número na lista"

# **Métodos

1. .append() para adicionar uma novo objeto na lista;
2. .clear() para limpar todos os valores da lista;
3. .copy() para copiar uma lista;
```python
numeros = [1,2,3,4,5,6]
n2 = numeros.copy()
```
4. .count() é usado para determinar quantas vezes um objeto aparece dentro de uma lista;
5. .extend() permite adicionar vários novos valores na lista (isso inclui juntar duas listas);
6. .index() informa em que índice está a primeira ocorrência de um objeto;
7. .pop() remove o último objeto da lista ou o objeto do índice indicado para ele;
8. .remove() remove o objeto diretamente. Você passa como argumento o objeto e não o índice onde ele está;
9. .reverse() inverte a ordem dos elementos da lista "in place" (sem criar nova lista);
10. .len() informa o tamanho do objeto que foi passado como argumento;
```python 
lista = ['Uva', 'Manga', 'Abacate']
len(lista) # 3
```

