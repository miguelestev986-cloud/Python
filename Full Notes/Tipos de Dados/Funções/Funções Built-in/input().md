04-12-25

State: #done

Tags: [[funções_built-in]]

----

# Para que serve

Ela é utilizada quando queremos ler dados da entrada padrão (teclado). Essa função sempre retorna uma string; se queremos outro tipo, precisamos converter explicitamente (int(), bool()...). 

----

# Parâmetros

Ela recebe um argumento opcional do tipo string, que é exibido para o usuário na saída padrão.

```python
alguma_coisa = input()
print(f"{alguma_coisa} é bem legal!")

>>>O que eu escrevo???
>>>O que eu escrevo??? é bem legal!
```

----

# Retorno

A função permite que o usuário escreva, e retorna a entrada ao chamador da função.

```python
nome = input("Qual a sua linguagem de programação?")
print(f"{nome} é uma ótima linguagem!")

>>>Qual a sua linguagem de programação? Python
>>>Python é uma ótima linguagem

# input retorna à função a string "Python"
```