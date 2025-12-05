04-12-25

Status: #done

Tags: [[instruções]]

----

# Conceito Geral

Tal qual break, temos o continue. Que *pula o resto do código da iteração atual* e inicia outra **iteração**.

```python
num = 0
while num < 500:
    if num == 369:
        num += 1
        continue
    print(num)
    num += 1

#Chega em 368 e pula para 370
```

----

# Referências
Bootcamp DIO [Suzano - Python Developer](https://www.dio.me/bootcamp/suzano-python-developer)
[[Iteração]]