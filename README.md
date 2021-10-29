# B_Tree
 A local implementation of a B_Tree
B-tree-Java implementation
Keywords: less

#Active insertion algorithm is adopted in this paper
-First, introduce B tree:
-B - tree is a self balanced search tree.
-In most other self balancing search trees, such as AVL and red black trees, it is assumed that everything is in main memory. To understand the use of b - trees, we have to consider large amounts of data that cannot be loaded into main memory. When the number of keys is high, the data is read from the disk in block form. Compared with main memory access time, disk access time is very high. The main idea of using b-tree is to reduce the number of disk accesses. Most tree operations (search, insert, delete, Max, min Etc.) requires O(h) disk access, where h is the height of the tree. b tree is a fat tree. Keep the height of b-tree low by placing the most possible key in the b-tree node.
-In general, the b-tree node size is equal to the disk block size. Because the H value of b-tree is low, compared with AVL tree, red black tree and other balanced binary search trees, the total disk access of most operations is greatly reduced. b - Tree Property
1) all leaves are at the same level. 
2) b-tree is defined by the minimum degree t. The value of T depends on the block size. 
3)  Each node, except the root node, must contain at least t-1 keys. The root directory can contain at least one key. All nodes (including the root node) can contain a maximum of 2t - 1 keys. 
5) The number of child nodes of a node is equal to the number of keys of the node plus 1.
6)  All keys of a node are sorted in ascending order. The subkeys between the two keys k1 and k2 contain all the keys in the range k1 and k2. Unlike binary search trees, b - trees grow and contract from the root. Binary search trees grow down and contract down.\
7) Like other balanced binary search trees, the time complexity of searching, inserting and deleting is O(Logn).
