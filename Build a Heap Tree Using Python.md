# Ex. No: 15D - Build a Heap Tree Using Python

## AIM:
To write a Python program to build a heap tree using appropriate Python package and function.

---

## ALGORITHM:

1. **Start the program.**
2. Import the `heapq` module.
3. Define a function `heaptree(H)` that takes a list `H` as input.
4. Use `heapq.heapify(H)` to convert the list into a min-heap.
5. Print the created heap.
6. **End the program.**

---

## PROGRAM:

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

<img width="1125" height="256" alt="image" src="https://github.com/user-attachments/assets/a7e81fe2-6108-4a93-8fc0-9cba1622fbe1" />
