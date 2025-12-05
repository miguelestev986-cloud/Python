05-12-25

State: #done

Tags: [[funções_built-in]]

----

# Para que serve

Usamos type para verificar o tipo primitivo de um valor.

----

# Parâmetros

Essa função possui três parâmetros. O uso mais comum, para verificar o tipo primitivo de um objeto, apenas o passamos como argumento.

```python
print(type("Amo pudim"))
print(type(10))
print(type(10.0))
print(type(True))

>>>str
>>>int
>>>float
>>>bool
```

Mas usando os três parâmetros, criamos uma dinâmica de classe. Neste uso, type() atua como um **metaclasse**, permitindo criar novas classes em tempo de execução.

```python
# 1. Corpo da classe (dicionário)
atributos = {
    'linguagem': "Python",
    'saudar': lambda self: "Olá!"
}

# 2. Criação da classe (nome, bases, corpo)
# A classe 'Pessoa' não herda de ninguém, então "bases" é ()
Pessoa = type('Pessoa', (), atributos)

# 3. Uso da classe criada dinamicamente
p = Pessoa()
print(p.linguagem)  # Saída: Python
print(p.saudar())   # Saída: Olá!
```

----

# Referências
[[Metaclasses]]
https://gemini.google.com/share/5bde0cb47eed