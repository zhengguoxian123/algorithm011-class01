学习笔记
#####1. 哈希表、映射、集合的实现与特性
set/map 查询O(1)
hash table 哈希表
hash function 哈希函数 
hash collisions 哈希碰撞 
完美哈希

优先队列 红黑树 AVL树
STL库已经实现好了，不需要大家手写，要掌握使用方式，API
查询 hash table C++
hash table 查询添加删除都是O(1)
![](https://upload-images.jianshu.io/upload_images/10106455-8493280c29bf2f6e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

工程上不使用哈希表，哈希表抽象出来的就是map和set(unordered_map/unordered_set)
map/set使用treeset,都是用红黑树来实现的，那么查询就是O(logN)(map/set)
![](https://upload-images.jianshu.io/upload_images/10106455-303a20b8546c44a2.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![](https://upload-images.jianshu.io/upload_images/10106455-42e62f74dc987737.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


#### 树、二叉树、二叉搜索树的实现和特性  要点
链表查询时间复杂O(n)
要加速就要升维度，那就变成树了
树和图最大的差别就是看有没有环 

##### 链表就是特殊化的树
##### 树就是特殊化的图，没有环的图就是树

树的遍历，前中后
拥抱递归
#### 第二周 第5课 | 哈希表、映射、集合 要点
##### 二叉搜索树
左子树的所有节点的值均小于他的根节点的值
右子树的所有节点的值均大于他的根节点的值
![](https://upload-images.jianshu.io/upload_images/10106455-7c305e7f8e3be36f.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![](https://upload-images.jianshu.io/upload_images/10106455-b6b8e2a160fecf04.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
树的遍历，因为是无序，所以是O(n)
二叉树要删除节点的话，如果删除的不是根节点，那么拿比他大或小的的最接近的来做垫背，一般取第一个大于他的节点
极端情况下，如下就变成一个链表，那么查询的复杂度就变成O(n)
![](https://upload-images.jianshu.io/upload_images/10106455-5ddd368eb742b3e4.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![](https://upload-images.jianshu.io/upload_images/10106455-d85afd30532d401c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
#### 把递归遍历记下来，变成肌肉记忆。
递归和动态规划难度比较大，学习比较陡峭
递归和循环效率都一样，不要把递归写残了，比如斐波那契数列
##### 二叉树各种遍历的迭代，看那个题解，都是用stack模拟操作!!!!!!统一解法!!!

#### 第二周 第6课 |  树、堆、图 要点
##### 堆和二叉堆的实现和特性
![](https://upload-images.jianshu.io/upload_images/10106455-4e11b693432ee1ff.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
数据结构怎么实现，堆的实现有很多种，比如二叉堆等，二叉堆只是相对比较容易实现，但时间复杂度刚刚及格
![](https://upload-images.jianshu.io/upload_images/10106455-a9d1b9b024661e11.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![](https://upload-images.jianshu.io/upload_images/10106455-748519cda2c14241.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
|完全二叉树|满二叉树|
-|-|
一棵深度为k的有n个结点的二叉树，对树中的结点按从上至下、从左到右的顺序进行编号，如果编号为i（1≤i≤n）的结点与满二叉树中编号为i的结点在二叉树中的位置相同，则这棵二叉树称为完全二叉树。|除最后一层无任何子节点外，每一层上的所有结点都有两个子结点的二叉树。|
如果用二叉搜索树实现堆的化，那么在find_min是O(logN)的。时间复杂度不合格。
![](https://upload-images.jianshu.io/upload_images/10106455-a3763ffbfc0e7116.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![](https://upload-images.jianshu.io/upload_images/10106455-ebfbcb22736fb3d7.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![](https://upload-images.jianshu.io/upload_images/10106455-e0cbec880154deff.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/10106455-a3775f57b4096e7a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
##### 记住二叉堆的性质
![](https://upload-images.jianshu.io/upload_images/10106455-c8e0d92a00eb3f4a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![](https://upload-images.jianshu.io/upload_images/10106455-6b980b46b02d9779.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/10106455-09e9bd29bcd303ed.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![](https://upload-images.jianshu.io/upload_images/10106455-c9da21e22537f05e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
优先队列是用堆来实现的，具体是用什么堆，有很多种，他是一个抽象的数据结构。二叉堆是一种常见且简单的实现，但是并不是最优的实现。

##### 3. 图的实现和特性
面试算法的话，基本上很少考图相关的东西
无/有向无/有权图
DFS和BFS这是面试经常考的，一般在树里考
![](https://upload-images.jianshu.io/upload_images/10106455-c12271f462d27649.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![递归是怎样的TODO](https://upload-images.jianshu.io/upload_images/10106455-4bd79f474c64e049.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
#### 代码模板一定要背诵下来！！！！一看到DFS、BFS就可以把模板咔咔咔写出来。变成条件反射，不要再花5分钟思考怎么写。然后再纸上慢慢调节，这样是不能接受的。
图用邻接矩阵/邻接表表示，邻接矩阵是什么
![临接矩阵是对称阵](https://upload-images.jianshu.io/upload_images/10106455-1032615d1275580a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![](https://upload-images.jianshu.io/upload_images/10106455-28ba0bc5c2462c40.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![](https://upload-images.jianshu.io/upload_images/10106455-f998371c08699eb1.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)







