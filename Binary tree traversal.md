
### Define a binary tree   
```
# Definition for a binary tree node.
  class TreeNode:
      def __init__(self, val=0, left=None, right=None):
          self.val = val
          self.left = left
          self.right = right
```

### Recursion method
1. parameters and return value for the recursion function (二叉树的parameter一般是node)
2. base case
3. determine the logic for a single-layer recursion

#### preorder
```
def preorderTraversal(self, root: Optional[TreeNode]) -> List[int]:

        def dfs(node):
            if node == None:
                return

            res.append(node.val) # root
            dfs(node.left) # left
            dfs(node.right) # right

        res = []
        dfs(root)
        return res
```

### Iteration method

   

