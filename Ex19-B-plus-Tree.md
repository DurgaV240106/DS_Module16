# Ex19 B+ Tree
## DATE:04-05-2025
## AIM:
To write a C function to traverse the elements in a B+ Tree.

## Algorithm
1.Start and loop through each element in the node’s data array.
2.If node is not a leaf, recursively traverse the current child before printing data.
3.Print the current data element.
4.After the loop, if node is not a leaf, traverse the last child pointer.
5.Return after completing traversal and end.
## Program:
```
/*
Program to traverse the elements in a B+ Tree.
Developed by: DURGA V
RegisterNumber: 212223230052 
*/

struct B_TreeNode
{
int *data;
structB_TreeNode**child_ptr;
int leaf;
int n;
};
structB_TreeNode*root =NULL, *np=NULL, *x=NULL;*/
void traverse(structB_TreeNode*p)
{
int i;
for(i=0;i<p->n;i++)
{
if(p->leaf==0)
{
traverse(p->child_ptr[i]);
}
printf("%d",p->data[i]);
}
if(p->leaf==0)
{
traverse(p->child_ptr[i]);
}
}
```

## Output:
![image](https://github.com/user-attachments/assets/69580512-f76d-4706-837b-4265c9f9fa1b)



## Result:
Thus, the function to traverse the elements in a B+ Tree is implemented successfully.
