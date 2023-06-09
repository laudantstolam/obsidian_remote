### Definition

>Heap sort 

一種Heap 的 sorting 方式，藉由比較父節點與子節點的大小來進行最大/最小heap的排列，max heap從最後的父節點開始判斷，與比其大(小)的子節點調換排列，直到root為最大/小的值為止。排序方式也可以分成top-down跟bottom-up兩種方式，top-down是一邊insert一邊調換，bottom-up是全部輸入完成再進行調換

>Binary Tree

一種樹狀架構，其中每個節點最多只有兩個分支(左子樹、右子樹)。二元樹的分支具有左右次序，不能隨意顛倒
- 每個 node 最多有兩個 subTree (也就是最多有兩個 child node)
- Left subTree (左子樹) 和 right subTree (右子樹) 是有順序的，順序不能任意顛倒
- 即使某個 node 只有一個 subTree，也必須區分它是 left subTree 還是 right subTree

>Binary Search Tree

1. 若任意節點的左子樹不空，則左子樹上所有節點的值均小於它的根節點的值；
2. 若任意節點的右子樹不空，則右子樹上所有節點的值均大於它的根節點的值；
3. 任意節點的左、右子樹也分別為二元搜尋樹；
具有上述性質的樹狀結構

>Heap

為⼀種完全⼆元樹，分為max/min heap兩種，其中max heap中所有⼦節點 內容必須比⽗節點⼩，故最⼤的數值必出現在root，min heap以此類推

>Binary Tree Traversal

遍曆二元樹的方法，分為preorder inprder postorder 分別事先左/右再讀取父節點

>Critical Path

中從開頭走到結尾所需經過的最長路徑，代表要消耗最多資源才能完成的線路
quick sort

![image.png](https://raw.githubusercontent.com/Ash0645/image_remote/main/202306191038909.png)
![image.png](https://raw.githubusercontent.com/Ash0645/image_remote/main/202306191040199.png)

https://z1nhouse.github.io/post/p0rM7JmKv/