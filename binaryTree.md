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

### 递归遍历二叉树

**use preorder traverse the binary tree**

```java

class Solution{
    public List<Integer> preorderTraverse(TreeNode root){
        List<Integer> res = new ArrayList<>();
        preorder(root, res);
        return res;
    }
    
    /** 前序遍历
    * 根节点->左孩子->右孩子
    */
    private void preorder(TreeNode root, List<Integer> res){
        // 递归终止条件为碰到空节点
        if(root == null) return;
        res.add(root.val);
        preorder(root.left, res);
        preorder(root.right, res);
    }
    
    /** 中序遍历
    * 左孩子->根节点->右孩子
    */
    private void inorder(TreeNode root, List<Integer> res){
        if(root == null) return;
        inorder(root.left, res);
        res.add(root.val);
        inorder(root.right, res);
        
    }
    
    /** 后序遍历
    * 左孩子->右孩子->根节点
    */
    private void backorder(TreeNode root, List<Integer> res){
        if(root == null) return;
        
    }
}
```




