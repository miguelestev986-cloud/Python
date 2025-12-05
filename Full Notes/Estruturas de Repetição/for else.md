04-12-25

Status: #done 

Tags: [[estruturas_repetição]]

----

# Conceito Geral

O **else** junto à **for** permite que um bloco de código seja executado quando o **iterável** de for se encerra normalmente (sem uso de **break**).

```python
for letra in 'Python':
	print(letra, end = ' ')
else:
	print('Acabou!')
>>>P y t h o n 
>>>Acabou!
```

```python
numeros = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
for num in numeros:
	print(letra, end = ' ')
	if num * 2 == 16:
		break
else:
	print('Acabou!')

>>>1 2 3 4 5 6 7 8
```
 
----

# Referências
Bootcamp DIO [Suzano - Python Developer](https://www.dio.me/bootcamp/suzano-python-developer)
[[Iteráveis]]
[[for]]
[[else]]