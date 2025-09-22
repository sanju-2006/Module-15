# Ex. No: 15A - height of the tree

## AIM:
Debug a Python function def heaptree(L): to build a tree and find out whether the tree is max heap and a complete tree, also print the height of the tree. 

Use appropriate module to build a binary tree.

---

## ALGORITHM:

1. **Start the program.**
2. **Import** the `Node` class from the `binarytree` module.
3. **Create a root node** using the `Node` class and assign a floating-point value.
4. **Create left and right child nodes** for the root with float values.
5. **Convert the tree** to a list and print the list of nodes.
6. **End the program.**

---

## PYTHON PROGRAM

```
from binarytree import heap,build,Node
def heaptree(L):
  x=L
  t=build(x)
  for i in t.values:
    print(i,"-->",end='')
  print("\nHeight : ",t.height)
  print("Is max heap? : ",t.is_max_heap)
  print("Is complete tree? : ",t.is_complete)
```

## OUTPUT
```
89 -->81 -->76 -->22 -->14 -->9 -->54 -->11 -->
Height :  3
Is max heap? :  True
Is complete tree? :  True
```

## RESULT

<img width="1137" height="236" alt="image" src="https://github.com/user-attachments/assets/40ab8fad-0d31-411c-b41a-dcc164cf7be6" />

