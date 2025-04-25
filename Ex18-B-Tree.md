# Ex4 (C) B-Tree
## DATE: 26/03/2025
## AIM:
To write a C function to delete an element in a B Tree.
## Algorithm
1. Start
2. Try to delete the item from the node using delValFromNode. If not found, print "Not present" and return.
3. If the node's count is 0 after deletion, set tmp to the current node and update myNode to its first linker child.Free the tmp node.
4. Update the global root to the new myNode.
5. Return after deletion.
6. End
 

## Program:
```
/*
/*
Program to write a C function to delete an element in a B Tree
Developed by: MOHAMED ARSHADULLAH A
RegisterNumber: 212224230161
*/
/*struct BTreeNode{
int item[MAX+1], count;
struct BTreeNode*linker[MAX+1];
};

struct BTreeNode*root;*/
voiddelete(int item, struct BTreeNode*myNode) { struct BTreeNode*tmp; if(!delValFromNode(item, myNode)){ printf("Not present\n");
return;
} else{
if(myNode->count ==0) { tmp = myNode;
myNode=myNode->linker[0]; free(tmp);
}
}
root=myNode; return;
}

*/
```

## Output:

![image](https://github.com/user-attachments/assets/43e954ce-5d91-4fdb-a830-da979111deb7)


## Result:
Thus, the C function to delete an element in a B Tree is implemented successfully.
