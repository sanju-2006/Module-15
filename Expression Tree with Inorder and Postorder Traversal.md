# Ex. No: 15C - Left and right node with string values

## AIM:
Write a python program to build a binary tree with a root,left and right node with string values

1. Use appropriate python library to build a binary tree using Node function

1. Get the node values (string) from the user and save it in a list

2. Print the list of nodes of the binary tree

---

## ALGORITHM:

1. **Start the program.**
2. Import the required modules (`build` and `Node` from `binarytree`).
3. Define a list `x` representing the expression tree in pre-order fashion (with `None` for missing nodes).
4. Use the `build()` function to generate the binary tree.
5. Print the **inorder** and **postorder** traversal of the tree.
6. **End the program.**

---

## PROGRAM:

```
from binarytree    import build
l=[]
for i in range(3):
    l.append(input())
root=build(l)
print(f"List of nodes : {list(root)}")
```

## OUTPUT

<img width="988" height="186" alt="image" src="https://github.com/user-attachments/assets/8dd85248-ec7d-4a01-a820-e1552d9896ec" />


## RESULT

 python program to build a binary tree with a root,left and right node with string values is successfully verified
