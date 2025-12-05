### Fontes
Bootcamp DIO [Suzano - Python Developer](https://www.dio.me/bootcamp/suzano-python-developer)
Curso em Vídeo Python - Mundo 1

# **O que são

*Variáveis* armazenam valores que nascem com um valor mas que podem sofrer alterações durante a execução do programa. Como o Python usa uma tipagem dinâmica (Define o tipo da variável pelo seu valor), logo não podemos declarar uma variável que não receba nenhum valor mas também não precisamos informar seu tipo. Para alterar o valor de uma variável, basta atribuir-lhe um novo valor.

```python 

nome = 'Calabreso da Silva'
#nome recebe Calabreso da Silva
idade = 20
#idade recebe 20
print(nome, idade)
```
Na saída (Tela): Calabreso da Silva 20

Podemos definir mais de uma variável em uma única linha:

```python

nome, idade = 'Calabreso da Silva', 20
print(f'Nome = {nome} Idade = {idade}')
```

# **Diferença entre elas

A diferença de uma variável para uma *constante* é que uma constante permanece com o valor definido inicialmente até o fim do programa (ou seja, o valor é imutável). Um detalhe é que o Python não tem uma palavra reservada para informar ao interpretador que o valor é constante, então por convenção as escrevemos em letras maiúsculas. Como constantes são como variáveis (apenas é entendido que o valor não mudará na execução do programa), os valores acabam podendo sim ser alterados na execução, diferente de outras linguagens.

# **Boas Práticas

- Os nomes não devem ter espaços(substitua-os por urderlines). Ex.: nome_da_variavel
- Os nome não devem ter acentos porque eles podem quebrar em alguns ambientes que não os suportam. 
- Escolha nomes sugestivos
- Escrevemos constantes em letras maiúsculas (para diferenciá-las de variáveis)