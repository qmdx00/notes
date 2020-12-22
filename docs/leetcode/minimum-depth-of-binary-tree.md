### 二叉树的最小深度

- 编号: 111
- 难度: 简单
- 描述: [minimum-depth-of-binary-tree](https://leetcode-cn.com/problems/minimum-depth-of-binary-tree/)

```java
class Solution {
    public int minDepth(TreeNode root) {
        if (root == null) return 0;
        int leftMin = minDepth(root.left);
        int rightMin = minDepth(root.right);

        return (leftMin == 0 || rightMin == 0)
                ? leftMin + rightMin + 1
                : Math.min(leftMin, rightMin) + 1;
    }
}

class TreeNode {
    int val;
    TreeNode left;
    TreeNode right;
    TreeNode(int x) {
        val = x;
    }
}
```
