# Data Engineer big data challenge



### Pergunta 1 - Qual é o retorno da chamada func1(14,60)?

```python
def func1(x, y):
  if y == 0:
    return 0
  
  elif y == 1:
    return x
  else:
    return x + func1(x, y-1)


print(func1(14, 60)) # 840
```

> ### uma forma mais simples de solucionar o problema seria: 14 x 60 = 840


### Pergunta 2 - Qual a complexidade computacional no número de adições para a função func1 chamada com x>0 e y>0?

> O(y)

---

> A função calculate abaixo aceita parâmetros de entrada a e b, os quais são dois parâmetros numéricos (int, float e complex).

````python
def calculate(a, b=None):
  try:
    if b:
      return a / b
    else: return a
  except:
    return a + b

print(calculate("b", "c"))

print(calculate(4, 2))

print(calculate(4))

print(calculate(4, 0))
````

> #### somente a afirmação I está correta

---

````python
class Shape():
  name = "shape"

  def __init__(self):
    self.color = "red"
  
  def perimeter(self):
    return self.height*2 + self.width*2

  def area(self):
    raise NotImplementedError()


class Square(Shape):

  def __init__(self, side):
    self.side = side
    super().__init__()

  def perimeter(self):
    return self.side * 4

  def area(self):
    return self.side**2


class Rectangle(Shape):
  name = "Rectangle"

  def __init__(self, height, width):
    self.height = height
    self.width = width

  def perimeter(self):
    return self.height*2 + self.width*2
````


### Pergunta 5 - Um(a) estagiário(a) deseja adicionar uma feature "minha_feature" a um repositório cujas branches "main" e "develop" são protegidas. Dentre as alternativas abaixo, qual comando ele(a) NÃO deve executar?

> "git merge feature/minha_feature" a partir da branch develop

---
 
### Pergunta 6 - A deleção do repositório local significa que é possível recuperar:

> Todas as modificações até o último push.


### Pergunta 7 - A modificação da outra pessoa na branch "develop" pode ter sido:


### Pergunta 8 - Qual a melhor alternativa para complementar o DDL acima e melhorar a performance de buscas mais gerais?

> Adicionar chaves primárias e estrangeiras nas colunas "id"


