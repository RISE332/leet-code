# binaryTree

## define a binaryTree node 

**use constructor function to create a binary tree node as follows:**

```java
public class TreeNode{
    int val;
    TreeNode left;
    TreeNode right;
    TreeNode() {}
    TreeNode(int val) {this.val = val;}
    TreeNode(int val, TreeNode left, TreeNode right) {
        this.val = val;
        this.left = left;
        this.right = right;
  }
}
```

**use preorder traverse the binary tree**
```java
class Solution{
    public List<Integer> preorderTraverse(TreeNode root){
        List<Integer> res = new ArrayList<>();
        preorder(root, res);
        return res;
    }
    
    private void preorder(TreeNode root, List<Integer> res){
        if(root == null) return;
        else{
            res.add(root.val);
            preorder(root.left, res);
            preorder(root.right, res);
        }
        
    }
}


```java



