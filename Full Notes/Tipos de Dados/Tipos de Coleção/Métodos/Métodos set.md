05-12-25

Status: #done

Tags: [[tipos_coleção]]

----

# Conceito

Podemos usar métodos para analisar e manipular conjuntos (**sets**)

----

# Métodos

union() retorna a união conjuntos;
```python
a = {1, 2}
b = {3, 4}
a.union(b) # {1, 2, 3, 4}
```

2. .intersection() retorna a intersecção dos conjuntos (partes que são comuns a ambos):
```python
a = {1, 2, 7, 4, 8}
b = {3, 4, 5, 2, 7}
a.intersection(b) # {2, 7, 4}
```

3. .difference()  retorna tudo que há em um conjunto que não há no outro:
```python
a = {1, 2, 3}
b = {3, 4}
a.difference(b) # {1, 2}
```

4. symmetric_difference()  retorna tudo que há fora da intersecção entre os conjuntos:
```python
a = {1, 2, 3}
b = {2, 3, 4}
a.symmetric_difference(b) # {1, 4}
```

5. .issubset() retorna True ou False para indicar se um conjunto é ou não um subconjunto de outro:
```python
a = {1, 2, 3, 4, 5}
b = {1, 2, 3, 4, 5, 6, 7, 8, 9}
a.issubset(b) # True
b.issubset(a) # False
# Todos os elementos de a estão em b, mas nem todos os elementos de b estão em a
```

6. .issuperset() é parecido com .issubset(), porque ele retorna True ou False para indicar se um conjunto tem todos os elementos do outro:
```python
a = {1, 2, 3, 4, 5}
b = {1, 2, 3, 4, 5, 6, 7, 8, 9}
a.issuperset(b) # False
b.issuperset(a) # True
```

7. .isdisjoint() retorna True ou False para indicar se os conjuntos não têm elementos em comum:
```python
a = {1, 2, 3, 4, 5}
b = {1, 2, 3, 4, 5, 6, 7, 8, 9}
c = {0, 10, 11}
a.isdisjoint(b) # False
b.isdisjoint(c) # True
```

8. .add() adiciona um valor caso esse já não exista dentro do conjunto:
```python
a = {1, 2, 3, 4, 5}
a.add(6) # {1, 2, 3, 4, 5, 6}
a.add(1) # {1, 2, 3, 4, 5, 6}
```

9. .clear() remove todos os elementos do conjunto;
10. .copy() cria uma cópia do conjunto;
11. .discard() descarta o valor indicado como argumento dentro do conjunto;
12. .pop() remove e retorna um elemento arbitrário do conjunto;
13. .remove() remove o objeto do conjunto mas, diferente de .discard(), ele dá erro se o objeto indicado não exista no conjunto;
14. len() informa o tamanho do conjunto que foi passado como argumento (len() é uma função embutida do Python, não um método especifico dos conjuntos);
15. in informa se o objeto à esquerda está no conjunto à direita:
```python
a = {1, 2, 3, 4, 5}
1 in a # True
6 in a # False
```

----
# Referências
[[set]]