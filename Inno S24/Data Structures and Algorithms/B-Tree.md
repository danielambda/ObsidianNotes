---
id: B-Tree
aliases: []
tags:
  - DataStructures
  - Algorithms
---
## Definition
1. Every node x has the following attributes:
    1. $x.n$ is the number of keys currently stored in node x
    2. The $x.n$ keys themselves, $x.key_1,x.key_2,...,x.key_{x.n}$, stored in monotonically increasing order, so that $\leq \leq \leq$
    3. $x.isLeaf$, a bool value that is true if x is a leaf
2. Each internal node x also contains $x.n + 1$ pointers $x.c_1, x.c_2,...,x.c_{x.n+1}$ to its children. Leaf nodes have no children, and so their $c_i$ attributes are undefined
3. The keys $x.key_i$ separate the ranges of leys stored in each subtree: if $k_i$ is any key stored in the subtree with root $x.c_i$, then $$k_1\leq x.key_1\leq k_2\leq x.key_2\leq...\leq x.key_{x.n}\leq k_{x.n+1}$$
4. All leaves have the same depth, which is the [[Tree]]'s height $h$
5. Nodes have lower and upper bounds on the number of keys they can contain, expressed in terms of a fixed integer $t\geq 2$ called the minimum degree of the B-Tree:
    1. Every node other than the root must have at least $t-1$ keys. Every internal node other than the root thus has at least $t$ children. If the tree is nonempty, the root must have at least one key.
    2. Every node may contain at most $2t-1$ keys. Therefore, an internal node may have at most $2t$ children. We say that a node is full if it contains exactly $2t-1$ keys
## Operations
```
search(key)
void create(BTree tree)
insert(key, value)
```
## Searching
- Searching a B-Tree is like searching a [[Binary Search Tree]], except that instead of making a binary branching decision at each node, the search makes a multiway branching decision according to the number of the node's children.
```cs
(Node Node, int Index)? BTreeSearch(Node x, Key k)
{
    int i = 0;
    while (i < x.n && k > x.keys[i])
        i++;

    if (i < x.n && k == x.keys[i])
        return (x, i)

    if x.IsLeaf
        return null;

    DiskRead(x.Children[i]);
    return BTreeSearch(x.Children[i], k);
}
```
## Creating
```cs
void CreateBTree(BTree tree)
{
    Node x = AllocateNode();
    x.IsLeaf = true;
    x.n = 0;

    DiskWrite(x);
    T.Root = x;
}
```
## Splitting Children
```cs
void BTreeSplitChild(Node x, int childIndex)
{
    Node nodeToSplit = x.Children[childIndex];
    Node newNode = AllocateNode();
    newNode.IsLeaf = nodeToSplit.IsLeaf;

    newNode.n = t - 1;

    for (int j = 0; j < t - 1; j++)
        newNode.Keys[i] = nodeToSplit.Keys[j + t];

    if (nodeToSplit.IsLeaf is false)
        for (int j = 0; j < t; j++)
            newNode.Children[j] = nodeToSplit.Children[j + t];

    nodeToSplit.n = t - 1;

    for (int j = x.n - 1; j >= childIndex; j--)
        x.Keys[j + 1] = x.Keys[j];

    x.Keys[childIndex] = nodeToSplit.Keys[t - 1];
    x.n++;

    DiskWrite(nodeToSplit);
    DiskWrite(newNode);
    DiskWrite(x);
}
```
## Insertion
```cs
void BTreeInsert(BTree tree, Key key)
{
    Node root = tree.Root;

    if (root.n == 2*t - 1)
    {
        Node newRoot = BTreeSplitRoot(tree);
        BTreeInsertNonfull(newRoot, key);

        return;
    }

    BTreeInsertNonfull(root, key);
}

Node BTreeSplitRoot(BTree tree)
{
    Node newRoot = AllocateNode();
    newRoot.IsLeaf = false;
    newRoot.n = 0;
    newRoot.Children[0] = tree.Root;
    tree.Root = newRoot;

    BTreeSplitChild(newNode, 0);
    return newNode;
}

void BTreeInsertNonfull(Node node, Key key)
{
    int i = node.Keys.Length - 1;

    if (node.IsLeaf)
    {
        while (i >= 0 && key < node.Keys[i]
        {
            node.Keys[i + 1] = node.Keys[i];
            i--;
        }

        node.Keys[i + 1] = key;
        node.n++;

        DiskWrite(node)
    }

    else
    {
        while (i >= 0 && key < node.Keys[i])
            i--;

        i++;
        DiskRead(node.Children[i]);
        if (node.Children[i].n == 2 * t - 1)
        {
            BTreeSplitChild(node, i);
            if (key > node.Keys[j])
                i++;
        }

        BTreeInsertNonfull(node.Children[i], key);
    }
}
```
