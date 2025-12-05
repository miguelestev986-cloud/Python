05-12-25

Status: #todo

Tags:

----

# Conceito

----

# Referências


### Fontes
Curso em Vídeo Python - Mundo 1
Bootcamp DIO [Suzano - Python Developer](https://www.dio.me/bootcamp/suzano-python-developer)
# **Fracionamento de Strings

O fracionamento de strings é uma técnica utilizada para retornar substrings (partes da string original), informando o início (start), o fim (stop) e o passo (step). Exemplos de uso:

1. 
```python
frase = 'Curso em Vídeo Python'
print(frase[1])
>>>u
```
O caractere 1 da frase é "u", porque o índice se inicia em 0.

2. 
```python
frase = 'Curso em Vídeo Python'
print(frase[0:5])

>>>Curso
```
"Curso" sem o espaço porque o stop não considera o último caractere. Também poderíamos omitir o zero, e o programa pegaria desde o início até o caractere que foi escolhido. 
Do mesmo modo, poderíamos omitir o final, e pegaria desde o caractere escolhido até o fim.

```python
frase = 'Curso em Vídeo Python'
print(frase[5:])

>>>em Vídeo Python
```
Na saída, teríamos: em Vídeo Python

3. 
Nesse exemplo, o programa pega desde o início até o fim,  saltando de 2 em 2 posições.
```python
frase = 'Curso em Vídeo Python'
print(frase[0:5:2])

>>>Cro
```
Porque pega os índices 0, 2 e 4.

4. Nós podemos usar números negativos para começar do fim para o início, assim como nesse exemplo: 

```python
frase = 'Curso em Vídeo Python'
print(frase[::-1])

>>>nohtyP odeíV me osruC
```
No exemplo, o step(-1) espelha a string porque pega os caracteres do final até o início (Já que nem o final nem o início são informados).
# **Análise de Strings

Algumas funções que podemos utilizar para analisar strings são:

1. len() verifica quantos caracteres a string tem;
2. .count('x') verifica quantas vezes o caractere 'x' aparece na string;
3. Com .count("x", 0, 14) podemos utilizar o fracionamento para verificar quantas vezes o caractere "x" aparece dentro de uma cadeia de caracteres.
4. .find('x') verifica em que caractere se inicia "x".  Se não há  "x" na string pertencente à variável, o programa nos devolve -1 ;
5.  'x' in nome_variável verifica se "x" existe na variável e nos devolve True ou False.
# **Transformação de Strings

Algumas funções que podemos utilizar para transformar strings são:

1. .replace('x', 'y') substitui "x" por "y" na string;
2. .upper() deixa todas as letras da string em letras maiúsculas;
3. .lower() transforma todas as letras da String em letras minúsculas;
4. .capitalize() põe o primeiro caractere da string em maiúsculo e deixa as outras em minúsculo;
5. .title() põe a primeira letra de cada palavra em maiúscula.
6. .strip() retira todos os espaços desnecessários da string;
7. De modo similar a .strip(), .rstrip() retira todos os espaços desnecessários do final (direita) da string e .lstrip() retira todos os espaços desnecessários do início (esquerda) da string.

# **Divisão e união de Strings

1. .split() separa as palavras (por meio dos espaços e brancos) e cria uma lista de strings com elas. Por exemplo:

```python
frase = 'Curso em Vídeo'
frases = frase.split()
print(frases[0])
```
Teríamos na saída: "Curso"

2. 'x'.join(nome_variável) junta os caracteres da string com o caractere "x".
3. .center(x, 'y') retorna uma nova string com preenchimento à esquerda e à direita, centralizando-a. Esse método possui dois argumentos: o primeiro define o número de caracteres da nova string e o segundo (que é opcional) define qual caractere vai ser usado na centralização. Ex.:

```python
curso = 'Python'
print(curso.center(10, '$'))
>>>$$Python$$
```

Caso você não informe o segundo argumento, ele centralizará com espaços em branco.

Uma observação é que os métodos retornam novas strings e não alteram a string original. Strings são imutáveis.

# **Interpolação de Variáveis

1. O método .format() é usado para formatar valores em uma string. Dentro dos parênteses são postos os valores que serão inseridos dentro das chaves. Ex.:

```python
nome = 'Davi Brito'
idade = 23
print('O nome do calabreso é {} e a idade dele é {}.'.format(nome, idade))

>>> O nome do calabreso é Davi Brito e a idade dele é 23.
```

Você também pode embaralhar e escolher a ordem dos valores:

```python
nome = 'Davi Brito'
idade = 23
print('O nome do calabreso é {1} e a idade dele é {0}.'.format(idade, nome))

>>> O nome do calabreso é Davi Brito e a idade dele é 23.
```
(O índice se inicia em 0)
Isso é útil quando a variável repete várias vezes na string, porque invés de repetir a variável várias nos argumentos do .format() basta por a mesma posição do índice.

2. String formatadas (f-strings) são uma forma moderna do método .format() porque deixa a string mais legível e simples. Ex.:

```python
nome = 'Davi Brito'
idade = 23
print(f'O nome do calabreso é {nome} e a idade dele é {idade}.')

>>> O nome do calabreso é Davi Brito e a idade dele é 23.
```

Com f-string podemos formatar os valores que serão substituídos. Ex.:

```python
PI = 3.14159
print(f'O valor de PI é {PI:2.2f}')

>>>O valor de Pi é  3.14
```
 O primeiro valor é a largura total e o segundo são as casas decimais

# **Strings de Múltiplas Linhas

Normalmente, nós usamos caracteres de escape como \t e \n para formatar strings que têm mais de uma linha, mas nós podemos usar strings triplas para isso. Elas formatam o texto assim como está na string, sem remover os espaços, quebra de linhas etc.

```python
print('\nO nome do curso é:\nPython')

>>>
O nome do curso é:
Python
```

```python
print('''
O nome do curso é:
	Python''')

>>>
O nome do curso é:
Python
```
Você pode usar tanto aspas simples(triplas) quanto duplas(triplas). Você pode usar f-strings assim sem problemas também:

```python
nome = 'Python'
print(f'''
O nome do curso é:
	{nome}''')

>>>
O nome do curso é:
Python
```