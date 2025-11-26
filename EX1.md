## Ex.No:1
## Ex.Name: check whether a tree is a Binary Search Tree or not and to traverse inorder
## Date:
## Aim:
To Write a C++ function to check whether a tree is a Binary Search Tree or not and to traverse inorder.

## Algorithm:
Start the program.

Define a Node structure with:

data (integer)

left and right pointers.

Create a function newNode(int val) to allocate a new node with the given value.

Create an insert(Node* root, int val) function to insert values into the BST:

If the tree is empty, create a new node.

If val < root->data, insert into the left subtree.

Else insert into the right subtree.

Create a function findMax(Node* root) to find the largest value:

Traverse right until root->right == NULL.

Return the node’s data.

In main():
Read number of nodes and their values.

Build the BST using insert().

Call findMax(root) and display the result.

Stop the program.

## Program:
```
void traverseInOrder(struct node *temp) {
  if (temp != NULL) {
    traverseInOrder(temp->left);
    cout << " " << temp->data;
    traverseInOrder(temp->right);
  }
}
```
## Output:

<img width="1237" height="807" alt="image" src="https://github.com/user-attachments/assets/c68551a2-c3ae-44ed-a83e-c9f2609488f4" />




## Result:
The Program Executed Successfully.
