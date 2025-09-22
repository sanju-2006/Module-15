# Ex. No: 15B - Build a Binary Search Tree Using Built-in Function

## AIM:
To write a Python program to build a binary search tree using a built-in function.

---

## ALGORITHM:

1. **Start the program.**
2. Define `_build_bst_from_sorted_values(sorted_values)` to recursively build a binary search tree (BST) from a sorted list.
3. Define `left_subtree(l)` to print the left subtree of the BST.
4. Take user input for the number of elements and store the values in a list `a`.
5. Sort the list and pass it to `_build_bst_from_sorted_values()` to construct the BST.
6. Print the postorder traversal of the BST.
7. Call `left_subtree(l)` to print the left subtree.
8. Check whether the tree is a binary search tree using the `is_bst` property.
9. **End the program.**

---

## PROGRAM:

```
from binarytree import Node

def _build_bst_from_sorted_values(sorted_values):
    if len(sorted_values)==0:
        return None
    mid_index=len(sorted_values)//2
    root=Node(sorted_values[mid_index])
    root.left=_build_bst_from_sorted_values(sorted_values[:mid_index])
    root.right=_build_bst_from_sorted_values(sorted_values[mid_index+1:])
    return (root)


def right_subtree(l):
    print("Right Subtree :")
    for i in l[2].values:
        print(i,"-->",end="")
    return

a=[]
size=int(input())
for i in range(0,size):
    val=int(input())
    a.append(val)
x=sorted(a)

l=_build_bst_from_sorted_values(x)
print("Postorder :",l.postorder)
right_subtree(l)
print("\nIs this a Binary Search Tree? ",l.is_bst)
```

## OUTPUT
```
Postorder : [Node(1), Node(3), Node(6), Node(4), Node(9), Node(12), Node(10), Node(8)]
Right Subtree :
10 -->9 -->12 -->
Is this a Binary Search Tree?  True
```

## RESULT


<img width="1120" height="550" alt="image" src="https://github.com/user-attachments/assets/059931d8-dbba-48f2-bebf-594103688e5d" />
