05-12-25

Status: #done

Tags: [[tipos_coleção]]

----

# Conceito

Podemos usar métodos para analisar e modificar listas (**list**)

----

# Métodos

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

----

# Referências
[[list]]