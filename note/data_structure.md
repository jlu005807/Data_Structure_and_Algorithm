# 绪论



## 数据结构的研究内容

### 数据结构主要研究**非数值计算问题 **

​           数据结构是一门研究**非数值计算**程序设计中的操作对象， 以及这些对象之间的关系和操作的学科。

> 例如:
>
> * 学生学籍管理系统
> * 人机对弈问题
> * 最短路径问题。





## 基本概念和术语



## 数据、 数据元素、 数据项和数据对象

### 数据（Date)

>数据 (Data) 是客观事物的符号表示，是所有能输入到计算机中并被计算机程序处理的**符号的总称**。
>
>* 数学计算中用到的整数和实数
>* 文本编辑中用到的字符串
>* 多媒体程序处理的图形、 图像、声音及动画等通过特殊编码定义后的数据

### 数据元素(Data Element)

>数据元素(Data Element)是数据的***基本单位***，在计算机中通常作为一个整体进行考虑和处理。 在有些情况下，数据元素也称为元素、记录等
>
>数据元素用千完整地描述一个对象
>
>* 一名学生记录
>* 树中棋盘的一个格局（状态）
>* 及图中的一个顶点

### 数据对象 (Data Object) 

> 数据对象 (Data Object) 是性质相同的数据元素的集合，是数据的一个子集。
>
> * 整数数据对象是集合N= {0, 士1' 士2,…}
> * 字母字符数据对象是集合C= {'A','B', …，'Z','a','b', …，  'z'}
> * 学生基本信息表也可以是一个数据对象

> 只要集合内元素的***性质均相同***，都可称之为一个数据对象。



## 数据结构

> 数据结构 (Data Structure) 是相互之间存在一种或多种**特定关系的数据元素的集合**。
>
> * 数据结构是带 ”结构＂ 的数据元素的**集合**
> *  “结构” 就是指数据元素之间存在的**关系**

### 逻辑结构

> 数据的逻辑结构是从**逻辑关系**上描述数据，它**与数据的存储无关**，是独立千计算机的。
>
> * 数据的逻辑结构可以看作是从具体问题抽象出来的**数学模型**。

> 数据的逻辑结构有两个要素
>
> * 数据元素
>
> * 关系  （指数据元素间的**逻辑关系**）
>
>   * 集合结构
>
>     > 数据元素之间除了 “**属于同一集合**” 的关系外，别无其他关系。例如，确定一名学生是否为 班级成员， 只需将班级看做一个集合结构。
>   * 线性结构
>     > 数据元素之间存在**一对一**的关系。例如，将学生信息数据按照其入学报到的时间先后顺序进 行排列，将组成一个线性结构。
>   * 树结构
>     > 数据元素之间存在**一对多**的关系。例如，在班级的管理体系中，班长管理多个组长，每位组长管理多名组员，从而构成树形结构。
>   * 图结构或网状结构
>     > 数据元素之间存在**多对多**的关系。例如，多位同学之间的朋友关系， 任何两位同学都可以是朋友，从而构成图状结构或网状结构。



#### 线性结构

> * 线性表（典型的线性结构，如例1.1中的学生基本信息表）
> * 栈和队列（具有特 4 l 第1章 绪论 I 殊限制的线性表，数据操作只能在表的一端或两端进行）
> * 字符串（也是特殊的线性表，其特殊性 表现在它的数据元素仅由一个字符组成）
> * 数组（是线性表的推广，它的数据元素是一个线性表）
> *  广义表（也是线性表的推广，它的数据元素是一个线性表，但不同构，即或者是单元素，或者是 线性表）

#### 非线性结构

>* 树（具有多个分支的层次结构）
>* 二叉树（具有两个分支的层次结构）
>* 有向图（一种图结构，边是顶点的有序对）
>* 无向图（另一种图结构，边是顶点的无序对）

### 存储结构

- 存储结构是逻辑结构在计算机中的存储表示
- 有两类存储结构：顺序存储结构和链式存储结构。

![image-20240716231256748](D:\Internt_of_Thing\e_book\数据结构和算法\note\assets\image-20240716231256748.png)



## 算法和算法分析

### 算法定义及其特性

- 算法 (Algorithm) 是为了解决某类问题而规定的一个**有限长的操作序列**。

- 算法由有限条指令构成，规定了解决特定问题的一系列操作。

- 一个算法必须满足以下五个重要特性。

  > 1. 有穷性：有限个步骤之后终止。
  > 2. 确定性：每条指令有明确的含义。
  > 3. 可行性：通过已经实现的基本运算执行有限次来完成。
  > 4. 输入：外界提供的量。
  > 5. 输出：结果。

### 评价算法优劣的基本标准

> 1. 正确性：正确结果
> 2. 可读性：
> 3. 健壮性（鲁棒性）：对有缺失、有噪声或有错误的输入数据，算法应具有较强的适应能力。
> 4. 高效性：时空复杂度。

### 时间复杂度

> - 影响算法时间代价的最主要因素是问题规模。
> - 问题规模是算法求解问题**输入量的多少**，是问题大小的本质表示，一般用整数n表示。
>
> - 一条语句的重复执行次数称作**语句频度**(FrequencyCount)
> - 而对于时间复杂度，取决于**基本运算**
> - 基本运算是指算法运行过程中起**主要作用且花费时间最多**的运算

### 空间复杂度

算法在实现时所需要的**辅助空间**



# 线性表

## 定义(逻辑结构)

- 由n(n>=0)个**数据特性相同**的元素构成的**有限序列**称为线性表

- 或者说是数据类型相同的元素组成的**有限集合**

- 线性表中元素的个数n(n>=0)定义为线性表的长度，n=0时称为**空表**。 

- 对千非空的线性表或线性结构，其特点是：

  > 1. 存在唯一的一个被称作“第一＂的数据元素；
  > 2. 存在唯一的一个被称作“最后一个＂的数据元素；
  > 3. 除第一个之外，结构中的每个数据元素均只有一个前驱；
  > 4. 除最后一个之外，结构中的每个数据元素均只有一个后继。

## 存储结构

### 顺序存储

- 线性表的**顺序表**示指的是用一组**地址连续的存储单元**依次存储线性表的数据元素，这种表示也称作线性表的顺序存储结构或顺序映像。
- 逻辑上相邻的数据元素，其物理次序也是相邻的
- 简单来说就是**数组**

### 链接存储

- 用**任意**一组存储单元存储线性表
- 一个存储单元除包含结点数据字段的值，还必须存放其逻辑相邻结点（前驱或 后继结点）的地址信息，即指针字段。
- **链表**

- **哨兵节点**：
  - 为便于在表头进行插入、删除操作，通常在表的前端增加一个特殊的**表头结点**，称其为哨位（哨兵）结点。

```cpp
//节点
struct ListNode{ 
 int data;
 ListNode* next;
 ListNode(int d){ data=d; next=NULL; }
 };

struct List{
    ListNode* headnode;//哨兵节点
}
```

 

### 时空效率比较

#### 空间

- 顺序表空间来自于申请的数组空间，数组大小确定，当元素较少时，顺序表中的很多空间处于闲置状态，造成了空间的浪费；
- 链表空间是根据需要动态申请的，不存在空间浪费问题，但链表需要在每个结点上附加一个指针，从而产生额外开销

#### 时间

|        | 基于下标的查找              | 插入/删除                   |
| ------ | --------------------------- | --------------------------- |
| 顺序表 | **O(1)**按下标直接查找      | **O(n)** 需要移动若干元素   |
| 链 表  | **O(n) **从表头开始遍历链表 | **O(1) **只需修改几个指针值 |



# 栈和队列

对于栈和队列，可以理解为**操作受限的线性表**，只可以在线性表的表头或者表尾进行操作

## 栈

### 定义

- 栈(stack)是限定仅在表尾进行插入或删除操作的线性表。
- 因此，对栈来说，表尾端有其特殊含义，称为栈顶(top)
- 相应地，表头端称为栈底(bottom)。
- 不含元素的空表称为空栈。
- 栈的修改是按后进先出的原则进行的，因此，栈又称为**后进先出(LastIn First Out, LIFO)**的线性表，

### 应用

- **进制转换**：假设十进制转换为K进制：

  > - 创建一个栈Stack
  > - 不断除以K取余数。后生成的余数先输出，先生成的余数后输出，正好符合栈的后进先出性质。

- **括号匹配**：
  > - 从左向右扫描字符串
  > - 若遇到左括号：压栈 
  > - 若遇到右括号：弹出栈顶的左括号与之匹配。
  > - 最后判断栈空
  
- n对括号共有多少种可能的**合法匹配序列**：第n个卡特兰数

  > `Cn=(2n)!/(n!*n!)/(n+1)`

- **表达式求值**：（中缀表达式转变为后缀表达式）

  > - 从左到右依次读入后缀表达式的每一个操作数/运算符/结束符
  > - 若读到的是操作数，将它压入栈。 
  > - 若读到的是运算符，就从操作数栈中连续弹出两个元素（操作数），进行相应的运算，并将结果压入栈中。 
  > - 读入结束符时，栈顶元素就是计算结果。

- **调度场算法**：中缀表达式转后缀表达式
  > - 设置一个栈，存放运算符从左到右依次读入中缀表达式的每一个元素
  > - 操作数规则：直接放入后缀表达式,注意对多位数的处理
  > - 运算符规则：
  >   - 栈空或栈顶是左括号：压栈
  >   - 当前运算符优先级>栈顶运算符：压栈
  >   - 当前运算符优先级<=栈顶运算符：弹栈直至当前运算符 优先级>栈顶或栈空或栈顶为左括号（期间弹出的运算符顺序依次放入后缀表达式），再把当前运算符压栈
  > - 括号规则： (1) 遇到左括号：压栈 (2) 遇到右括号：弹栈直至左括号 
  > - 结束符规则：弹栈至栈空
  
- **栈混洗**：给定入栈序列，模拟出栈序列

  > - n个元素的栈混洗总数，即n对括号的匹配序列，卡特兰数*(n+1)
  >
  > - n个元素的栈混洗合法出栈序列，即n对括号的合法匹配序列，卡特兰数*(n+1)

- 利用**栈模拟队列**:

  > 利用两个栈模拟队列

- 共享栈

## 队列

### 定义

- 队列(queue)是一种**先进先出(First In First Out, FIFO)**的线性表
- 允许插入的一端称为队尾(rear), 允许删除的一端则称为队头(front)。

### 应用

- BFS广度优先搜索

- 栈和队列都需要注意的一点是top和rear指针是**指向元素还是下一个空位置**，判满和判空条件不同，

- 双端队列



# 数组和矩阵

## 数组

### 多维数组的存储和寻址：

- 已知数组`A[a][b][c][d]`,每个元素占C个存储单元
-  数组元素`A[i] j][k][l]`的存储地址：
  - 行优先:`Loc(A)+( i*b*c*d + j*b*d + k*d + l )*C`
  - 列优先:`Loc(A)+( i + j*a + k*a*b + l*a*b*c )*C`

### 矩阵的压缩存储

- 压缩存储需考虑2个问题
  - 需要多大存储空间：数组d[ ]需要多少元素 
  - 地址映射：矩阵的任意元素M(i, j)在一维数组d[ ]中的位置（下标）， 即把矩阵元素的下标映射到数组d的下标


1. **对角矩阵的压缩存储**
   1. 对于一个n*n的对角矩阵，至多只有n个非0元素，因此只需存储n个对角元素
   2. `M( i , i ) -> d[ i ]`

2. **(下）三角矩阵的压缩存储**
   1. 以按行优先方式压缩存放在一维数组d，d需要`n(n+1)/2`个元素
   2. `M(i, j)= d[k]=d[i(i−1)/2 + (j−1)]`

3. **对称矩阵M**的压缩存储
   
   1. 对称矩阵中M(i, j)与M(j, i)的信息相同，只需存储M的下三角部分的元素信息。
   2. 对于对称矩阵中的下三角元素`M(i, j) (i>=j)` :
      1. `i < j，M(i, j)=d[k]，k = i(i−1)/2 + (j−1)`
   3. 对于上三角元素`M(i, j) (i<j)`:元素值与下三角矩阵中的 元素M(j,i)相同
      1. `i < j, M(i, j)=M(j, i)=d[q]， q= j(j−1)/2 + (i−1)`
   
4. **三对角矩阵M的压缩存储**
   
   1. 方阵Mn*n中任意元素M(i, j)，当| i - j | >1时，有M(i, j) =0， 则 M称为三对角矩阵。
   2. 需要3*n-2个存储单位
   3. 对于非零元素：即`| i-j | <=1, M(i,j) = d[2*i + j - 3]`
   
5. 稀疏矩阵的压缩存储

   1. 非零元素的个数远小于零元素的个数
   2. 三元组结点来存储矩阵的每个非零元素aij，其中i和j为元素的行号和列号，即`node(i,j,aij)`
   
      ```cpp
      struct Triple{
          int row;
          int col;
          int value;
       };
      
       Triple Array[100];
      ```
   
      - 对于三元组有一个需要注意的算法：**稀疏矩阵的快速转置**。
      - 预先确定矩阵M中每一列（即T中每一行）的第一个非零元的位置
      - 求出每行非零元素个数，然后利用`cpot[col]=copt[col-1]+num[col-1]`，求出位置
   
   3. 十字链表:`数据,该结点所在行 ,该结点所在列 ,指向左侧相邻非零元素的指针 ,指向上方相邻非零元素的指针`,即`node(row,col,value,left,up)`
   
      ```cpp
       struct ListNode{
          int row; //节点所在行
          int col; //节点所在列
          int value; //数据
          ListNode* left;//指向左侧相邻非零元素的指针
          ListNode* up; //指向上方相邻非零元素的指针
       };
      ```
   
      
   
   4. 双向十字链表：在十字链表的基础上增加双方向的指针，并有循环链表的特点
   
      ```cpp
       struct ListNode{
          int row; //节点所在行
          int col; //节点所在列
          int value; //数据
          ListNode* left;//指向左侧相邻非零元素的指针
          ListNode* up; //指向上方相邻非零元素的指针
          ListNode* right; //指向右侧相邻非零元素的指针
          ListNode* down;  //指向下方相邻非零元素的指针
       };
      ```
   
      
   
   

# 字符串

## 定义

- 串(string)(或字符串）是由零个或多个字符组成的**有限序列**
- 串中字符的数目n称为串的长度
- 零个字符的串称为空串(null string) , 其长度为零

## 应用

- 模式匹配：

  - 朴素模式匹配：经典的暴力匹配算法实现（BF算法）

  ```cpp
  int BF(std::string S, std::string T, int pos)
  {
      // 检查pos是否合法，pos小于0或pos+T的长度超过S的长度都返回-1
      if (pos < 0 || pos + T.size() > S.size())
      {
          return -1; // pos错误
      }
  
      // 初始化i为搜索起始位置，j为T中正在匹配的字符位置
      int i = pos;
      int j = 0;
  
      // 开始匹配，直到S或T遍历完
      while (i < S.size() && j < T.size()) 
      {
          // 如果S[i]和T[j]字符相等，则继续向后匹配
          if (S[i] == T[j])
          {
              i++;  // S指针后移
              j++;  // T指针后移
          }
          else // 如果不匹配，回溯i，并从T的开头重新开始匹配
          {
              i = i - j + 1;  // i回溯到匹配失败后的位置
              j = 0;  // T重新从头开始匹配
          }
      }
  
      // 如果j已经匹配到T的末尾，则说明匹配成功，返回匹配的起始位置
      if (j >= T.size())
      {
          return i - T.size();  // 返回匹配成功的位置
      }
      else // 如果没有完全匹配，返回-1表示匹配失败
      {
          return -1;
      }
  }
  ```

  

  - KMP:
    - 利用“部分匹配表”（即 `next` 数组）来优化暴力匹配的过程，避免了不必要的字符比较,重点就在于next数组的创建
  
  
  ```cpp
  int index(std::string S, std::string T, int pos)
  {
      // 创建一个shared_ptr动态数组用于存储T的next数组
      std::shared_ptr<int[]> next(new int[T.size()], std::default_delete<int[]>());
  
      // 计算T的next数组
      get_next(T, next);
  
      // 初始化i, j为匹配指针，i指向S，j指向T
      int i = 0;
      int j = 0;
  
      // 获取S和T的长度
      int sl = S.size();
      int tl = T.size();
  
      // KMP匹配过程：若字符匹配成功（S[i] == T[j]），或者j == -1（表示跳过不匹配的字符），则继续比较下一个字符
      while (i < sl && j < tl)
      {
          if (j == -1 || S[i] == T[j]) // 如果j == -1或字符匹配，则i和j都加1
          {
              i++;
              j++;
          }
          else // 如果字符不匹配，且j != -1，则根据next数组调整j的位置
          {
              j = next[j]; // 将j跳到next[j]的位置，避免不必要的字符比较
          }
  
          // Debug代码：输出匹配过程中的状态
          /*std::cout << S.size() << " " << T.size() << std::endl;
          std::cout << i << " " << j << std::endl;
          if (j < T.size()) { std::cout << "ozy"; }
          system("Pause");*/
      }
  
      // 如果j达到了T的末尾，说明匹配成功，返回匹配的起始位置
      if (j == T.size())
      {
          return i - T.size();  // 返回匹配开始的位置
      }
      else // 如果j未能到达T的末尾，说明匹配失败，返回-1
      {
          return -1;
      }
  }
  
  // 计算字符串T的next数组
  void get_next(std::string T, std::shared_ptr<int[]>& next)
  {
      next[0] = -1;  // next数组的第一个位置默认是-1
      int k = -1;     // k表示当前最长前后缀的长度
      int j = 0;      // j用于遍历T字符串的字符
  
      // 计算T字符串的next数组，构建部分匹配表
      while (j < T.size() - 1) // 注意这里j < T.size() - 1，避免越界
      {
          // 如果k == -1表示没有匹配的前后缀，或者T[j]和T[k]相等
          if (k == -1 || T[j] == T[k])
          {
              ++k;  // 扩大前缀长度
              ++j;  // 移动j，继续处理下一个字符
              next[j] = k;  // 将当前j的next值设为k
          }
          else // 如果T[j]与T[k]不相等，根据next数组递归查找更短的前后缀
          {
              k = next[k];  // 将k回退到next[k]的位置
          }
      }
  }
  
  ```

  
  
  - 注意next数组的意义以及和失败函数fail的区别:
    - `next[j] = fail[j-1]+1`
    - next[j]为在string[0,j-1]子字串的最大相等前后缀的长度加一，即**跳转的位置**
    - fail[j]为string[0,j]子字串的最大相等前后缀的长度。
    - 对于next数组的优化：如果跳转位置的字符`string[ next[j] ]`和`string[j]`相同，即跳转后依旧匹配失败继续跳转，所以可以将`next[j]=next[ next[j] ]`。



# 树

## 定义

- 一棵树是结点的一个有限集合T。

- 若T空，则称为空树。 

- 若T非空，则：
  - 有一个被称为根的结点，记 为`root(T) `； 
  - 其余结点被分成m(m >=0) 个 不相交的非空集合T1,T,…,Tm， 且T1, T2, …, Tm也都是树，其 称为`root(T)`的**子树**。(递归结构)
  
- 相关术语
  > - 度 ：一个结点的度指该结点的子结点的数目。其中一棵树的度为各结点的度的最大值。
  > - 叶结点：度为0的结点，即没有孩子节点的结点。
  > - 分支结点 ：度大于0的结点，即非叶结点
  > - 边：树中结点间的连线
  > - 层数/深度：根结点层数为0，其余结点的层数为其父结点的层数加1。
  > - 树的高度/深度：树中结点的最大层数
  > - 结点的高度：以该结点为根的子树的高度
  
- 对于二叉树

  > - 二叉树中第i层至多有2^i个结点，i>=0
  > - 高度为k的二叉树中至多有`2^(k+1)-1 (k>=0)`个结点
  > - 在n个结点构成的二叉树中，若叶结点即度为零的结点个数为n0 ，度为2的结点个数为n2 ，则有：`n0 = n2 ＋1`
  > - 特殊二叉树
  >   - 完全二叉树：
  >     - 除最下一层外，每一层都是满的（达到 最大结点数），
  >     - 最后一层结点从左至右出现
  >     - 对所有结点，按层次顺序从1开始编号，仅编号最大的非叶结点可以没有右孩子，其余非叶结点都有两个子结点
  >     - 知道总度数可以求出各个不同度的节点数，因为度为1只可以为`0或者1`
  >   - 满二叉树（特殊的完全二叉树）：
  >     - 叶节点都在最后一层
  >     - 每个非叶节点都有两个子节点

## 存储结构

### 顺序结构

将树的结点存放在数组里

或者我们这需要关注**各个结点的逻辑关系**而非各个结点的数据时，可用int数组,例如：对于第i个结点，父节点为tree[i]，特殊的根节点的没有父节点所以对应的值为本身或者一个负数，这个用法可用于哈夫曼树或者并查集

- 根节点存放在tree[0]，则`tree[i]`对应的左右子树分别为`tree[2*i+1]`,`tree[2*i+2]`，父节点为`tree[(i-1)/2](i>=1)`
- 根节点存放在tree[1]，则`tree[i]`对应的左右子树分别为`tree[2*i]`,`tree[2*i+1]`父节点为`tree[i/2]（i>0)`
- 比较适用于满二叉树和完全二叉树，对于普通的树未使用的空间较多

``` cpp
template<class T>
class Complete_BiTree
{
public:
	std::vector<T> tree;
};
```

### 链接存储

利用指针用类似链表的方式连接各个结点

```cpp
template<class T>
class BiTree
{
public:
	T data;//数据

	BiTree<T>* parent;//父节点,可有可无
	BiTree<T>* leftChild;//左子树
	BiTree<T>* rightChild;//右子树

	//左右子树是否为线索
	bool leftTag;
	bool rightTag;

	BiTree() = default;
};
```

### 重要操作

- 树的遍历（以链接存储为例）

  二叉树的遍历：按照一定次序访问二叉树中所有结点， 并且每个结点仅被访问一次的过程

  - 前序遍历(类似图的深度优先搜索DFS)，利用栈可以实现非递归。

    ```cpp
    //这里function不一定返回空，具体视情况而立,默认为输出data
    	void PreOrderTraverseTree(BiTree<T>* tree,/*处理函数*/std::function<void(T&)> address = [](T& e)->void {std::cout << e; })
    	{
    		//空树
    		if (!tree)
    		{
    			return;
    		}
    
    		//根节点
    		address(tree->data);
    
    		//遍历左子树
    		if (tree->leftChild && !tree->leftTag)
    		{
    			PreOrderTraverseTree(tree->leftChild, address);
    		}
    
    		//遍历右子树
    		if (tree->rightChild && !tree->rightTag)
    		{
    			PreOrderTraverseTree(tree->rightChild, address);
    		}
    
    		return;
    
    	}
    
    ```

    - 非递归

      ```cpp
      // 非递归前序遍历函数，使用栈模拟递归过程
      void Non_Recursive_PreOrderTraverseTree(BiTree<T>* tree,/*处理函数*/std::function<void(T&)> address = [](T& e)->void {std::cout << e; })
      {
          // 空树情况，直接返回
          if (!tree)
          {
              return;
          }
      
          // 初始化栈，用于保存遍历过程中的结点
          std::vector<BiTree<T>*> stack;
      
          BiTree<T>* current = tree; // 当前结点指向树的根结点
          
          // 当前结点非空或者栈非空时，继续遍历
          while (current || !stack.empty())
          {
              // 遍历到当前结点时
              if(current)
              {
                  // 处理当前结点（例如打印当前结点的数据）
                  address(current->data);
      
                  // 将当前结点压入栈中，以便后续回溯
                  stack.push_back(current);
      
                  // 转向当前结点的左子树继续遍历
                  current = current->leftChild;
              }
      
              // 当前结点为空但栈不为空时，需要回溯
              else
              {
                  // 从栈中弹出一个结点，恢复到上一个结点
                  current = stack.back();
      
                  // 弹出栈顶结点
                  stack.pop_back();
      
                  // 转向当前结点的右子树继续遍历
                  current = current->rightChild;
              }
          }
      }
      
      ```

      

  - 中序遍历，利用栈实现非递归。

    ```cpp
    void InOrderTraverseTree(BiTree<T>* tree,/*处理函数*/std::function<void(T&)> address = [](T& e)->void {std::cout << e; })
    	{
    		//空树
    		if (!tree)
    		{
    			return;
    		}
    
    		//遍历左子树
    		if (tree->leftChild && !tree->leftTag)
    		{
    			InOrderTraverseTree(tree->leftChild, address);
    		}
    
    		//根节点
    		address(tree->data);
    
    		//遍历右子树
    		if (tree->rightChild && !tree->rightTag)
    		{
    			InOrderTraverseTree(tree->rightChild, address);
    		}
    
    		return;
    
    	}
    ```

    - 非递归

    ```cpp
    // 非递归中序遍历函数，使用栈模拟递归过程
    void Non_Recursive_InOrderTraverseTree(BiTree<T>* tree, /*处理函数*/std::function<void(T&)> address = [](T& e)->void {std::cout << e; })
    {
        // 空树情况，直接返回
        if (!tree)
        {
            return;
        }
    
        // 初始化栈，用于保存遍历过程中的结点
        std::vector<BiTree<T>*> stack;
    
        BiTree<T>* current = tree; // 当前结点指向树的根结点
    
        // 当前结点非空或者栈非空时，继续遍历
        while (current || !stack.empty())
        {
            // 遍历到当前结点的左子树
            if (current)
            {
                // 将当前结点压入栈中，以便后续回溯
                stack.push_back(current);
                // 转向左子树继续遍历
                current = current->leftChild;
            }
    
            // 当前结点为空但栈不为空时，需要回溯
            else if (!stack.empty())
            {
                // 从栈中弹出一个结点，恢复到上一个结点
                current = stack.back();
                // 弹出栈顶结点
                stack.pop_back();
    
                // 处理当前结点（例如打印当前结点的数据）
                address(current->data);
    
                // 转向当前结点的右子树继续遍历
                current = current->rightChild;
            }
        }
    }
    
    ```

    

  - 后序遍历

    ```cpp
    void PostOrderTraverseTree(BiTree<T>* tree,/*处理函数*/std::function<void(T&)> address = [](T& e)->void {std::cout << e; })
    	{
    		//空树
    		if (!tree)
    		{
    			return;
    		}
    
    		//遍历左子树
    		if (tree->leftChild && !tree->leftTag)
    		{
    			InOrderTraverseTree(tree->leftChild, address);
    		}
    
    		//遍历右子树
    		if (tree->rightChild && !tree->rightTag)
    		{
    			InOrderTraverseTree(tree->rightChild, address);
    		}
    
    		//根节点
    		address(tree->data);
    
    		return;
    
    	}
    ```

    - 非递归

    ```cpp
    void Non_Recursive_PostOrderTraverseTree(BiTree<T>* tree, /*处理函数*/ std::function<void(T&)> address = [](T& e)->void { std::cout << e; })
    {
        // 空树情况，直接返回
        if (!tree)
        {
            return;
        }
    
        // 初始化栈，用于保存遍历过程中的结点
        std::vector<BiTree<T>*> stack;
    
        BiTree<T>* current = tree; // 当前结点指向树的根结点
        BiTree<T>* lastVisite = nullptr; // 记录上一个被访问的结点，用于判断右子树是否已访问
    
        // 当前结点非空或者栈非空时，继续遍历
        while (current || !stack.empty())
        {
            // 遍历到当前结点的左子树
            if (current)
            {
                stack.push_back(current); // 将当前结点压入栈中
                current = current->leftChild; // 转向左子树
            }
            else
            {
                // 当前结点为空，回溯到栈顶结点
                BiTree<T>* top = stack.back();
    
                // 如果右子树存在且未访问，则遍历右子树
                if (top->rightChild && lastVisite != top->rightChild)
                {
                    current = top->rightChild; // 转向右子树
                }
                else
                {
                    // 右子树为空或者已访问
                    address(top->data); // 处理当前结点
                    lastVisite = top; // 更新上一个访问的结点
    
                    stack.pop_back(); // 弹出栈顶结点
                }
            }
        }
    }
    
    ```
    
    
    
    - 层次遍历（类似图的广度优先搜索BFS）
    
      ```cpp
      void LevelOrderTraverseTree(BiTree<T>* tree,/*处理函数*/std::function<void(T&)> address = [](T& e)->void {std::cout << e; })
      	{
      		//空树
      		if (!tree)
      		{
      			return;
      		}
      
      		std::queue<BiTree<T>*> trees;
      		trees.push(tree);
      
      		while (!trees.empty())
      		{
      			BiTree<T>* p = trees.front();
      			trees.pop();
      
      			address(p->data);
      
      			//左子树
      			if (p->leftChild && !p->leftTag)
      			{
      				trees.push(p->leftChild);
      			}
      
      			//遍历右子树
      			if (p->rightChild && !p->rightTag)
      			{
      				trees.push(p->rightChild);
      			}
      
      		}
      		return;
      
      	}
      ```
    

- 树和二叉树的转换（**树使用兄弟儿子表示法**）

## 应用

- 先根序列个数为n的不同二叉树的个数为**卡特兰数**

- 线索二叉树：利用**节点的空指针**指向结点的某个序列的前驱和后继

- 哈夫曼树
  
  - 构造
  
    > - 一类带权路径长度最短的树。（用于不等长最优编码等）
    > - 在哈夫曼树中，权值越大的结点离根结点越近。
    > - 依次找到最小的两个节点组成一棵树直到所有节点都有根节点
  
  - 编码：
  
    > - 在构造哈夫曼树之后，求哈夫曼编码的主要思想是：依次以叶子为出发点，向上回溯至根结点为止。 
    > - 回溯时走左分支则生成代码 0, 走右分支则生成代码 l
  
  - 译码：
  
    > - **初始化**：从根节点开始，遍历二进制编码字符串。
    >
    > - **遍历路径**：
    >   - 每个`'0'`表示向左子树移动，`'1'`表示向右子树移动。
    >   - 每当到达叶子节点，就记录该节点编号即译出一个字符，并重新从根节点开始译码。
    >
    > - **结束判断**：若最终到达叶子节点，返回所有编号；否则该串无法译码为非法序列。
    >
    > 
  
- 并查集
  - 一种用于管理元素所属集合的数据结构，实现为一个森林

  - 其中每棵树表示一个集合，树中的节点表示对应集合中的元素。

  - 优化搜索

    > - 压缩路径
    >   - 查询过程中经过的每个元素都属于该集合，我们可以将其直接连到根节点以加快后续查询。
    >
    > ```cpp
    > size_t find(size_t x)
    > 	{
    > 		return pa[x] == x ? x : pa[x]=find(pa[x]);
    > 	}
    > ```
    >
    > - 小树并入大树(按秩合并)
    >
    > ```cpp
    > // 合并两个集合，x 和 y 所在的集合进行合并，按秩合并策略
    > size_t unite(size_t x, size_t y)
    > {
    >     // 找到 x 和 y 所在集合的根节点
    >     x = find(x);
    >     y = find(y);
    > 
    >     // 如果 x 和 y 已经在同一个集合中，无需合并，直接返回
    >     if (x == y) return;
    > 
    >     // 按秩合并，始终将小树合并到大树上
    >     // 如果 x 的树小于 y 的树，将 x 和 y 交换，确保 x 是较大的树的根
    >     if (size[x] < size[y])
    >     {
    >         std::swap(x, y); // 交换 x 和 y，确保 x 是较大的树根
    >     }
    > 
    >     // 将 y 的根节点合并到 x 的根节点
    >     pa[y] = x;  // 更新父节点数组，将 y 的父节点设为 x，表示 y 的根节点为 x
    > 
    >     // 更新 x 所在树的大小，将 x 的集合大小加上 y 集合的大小
    >     size[x] += size[y]; // size[x] 累加 size[y]，更新 x 集合的大小
    > }
    > 
    > ```

    - 集合数：如果一个节点的根指向自己，则为整棵树的根即一个集合。





# 图

## 定义

图(Graph) G由两个集合V和E组成，记为G=(V,E) , 其中V是顶点的有穷非空集合， E是V中顶点偶对的有穷集合，这些顶点偶对称为边。

## 存储结构

- 边存储

  将各个点的关系利用边存起来

  ```cpp
  struct Edge
  {
  	//存储边节点的编号
  	//u->v
  	int u;
  	int v;
  
  	//加入权值
  	int weight;
  
  	Edge() = default;
  
  	Edge(int _u, int _v,int weight=1) :u(_u), v(_v),weight(weight){	}
  };
  
  ```
  
  

- 邻接表（稀疏图）

  用顶点表将各个邻接点利用链接结构存放起来

  ```cpp
  //边结点
  //边链表中边结点包括邻接点域(adjvex)、数据域(info) 和链域(nextarc) 三部分
  //邻接点域指示与顶点V; 邻接的点在图中的位置；数据域存储和边相关的信息， 如权值等；链域指示与顶点v邻接的下一条边的结点。
  template<class T=int>//默认为int
  class ArcNode
  {
  public:
  	//该边所指向的顶点位置，如果为有向边则为弧头
  	int adjvex;
  
  	//指向下一条边的指针
  	std::shared_ptr<ArcNode<T>> nextarc;
  
  	//边信息，如权值,默认无信息
  	T info;
  
  	ArcNode() = default;
  
  	ArcNode(int vex) :adjvex(vex),info(1),nextarc(nullptr){ }
  
  	ArcNode(int vex,T info) :adjvex(vex),info(info), nextarc(nullptr) { }
  
  };
  
  template<class K = int, class T = int>
  class Adj_List
  {
  public:
  	//表头结点表，此vector.size()即顶点数,所以不需要记录顶点数
  	std::vector<VexNode<K, T>> vertices;
  
  	//记录边数
  	int arcnum;
  
  	//是否为有向图
  	bool is_direct;
  };
  ```

  - 对于链式结构的的邻接表，可以使用变为使用数组存放边的**前向星**

  ```cpp
  // 边类定义，包含两个成员变量：目标节点v和权重w
  class edge
  {
  public:
      int v;  // 目标节点
      int w;  // 边的权重
  
      // 构造函数，初始化目标节点和边的权重
      edge(int _v, int _w) :v(_v), w(_w){ }
  };
  
  // 存储图的邻接表(前向星)，vextices[i]表示节点i的所有边
  vector<vector<edge>> vextices;
  
  ```

  

- 邻接矩阵（稠密图）

  - 利用矩阵(即二维数组）将各个点是否存在边的信息存放起来


```cpp
//使用一个二维数组 adj 来存边，其中 adj[u][v] 为 1 表示存在 u 到 v 的边，为 0 表示不存在。
//如果是带边权的图，可以在 adj[u][v] 中存储 u 到 v 的边的边权。
//默认顶点到自身没有边
//并且二维数组难以改变结构所以不考虑增加和删除节点但是可以增删边，并且二维数组空间大不适用于稀疏图
//其实无向图为对称矩阵可以压缩为一维数组存放，但是实现逻辑相似不考虑分离  
//小技巧：对于有向无向图图，并且规定没有弧为0，有弧为1，则矩阵A^n[i][j]的值表示从顶点i到顶点j中路径长度为n的数目

class Adj_Matrix
{
public:
	std::vector<std::vector<int>> graph;

	//标志是否为有向图
	bool is_direct;

	Adj_Matrix() = default;

	//顶点数量number,依旧从零开始,当weight默认时表示无权图
	Adj_Matrix(int number,bool direct=false, int weight = INT_MAX):is_direct(direct)
	{
		graph.resize(number, std::vector<int>(number,weight));
	}
};

```

- 对于邻接表和邻接矩阵的比较
  - 首先是，邻接表适用于稀疏图，邻接矩阵适用于稠密图
  - 判断两个顶点是否存在边或者查询修改边的信息，邻接表O(n)（n表示该点的出度），邻接矩阵O(1)，所以频繁查询和修改边的信息则邻接矩阵更合适
  - 对于需要增删顶点则邻接表更适合

## 应用(重要操作)

都以邻接矩阵为例

- DFS:深度优先搜索，非递归时使用栈

```cpp
//深度优先搜索（DFS）算法,并对节点进行处理,vis保存是否访问
	void dfs(int u, std::vector<bool>& vis, const Adj_Matrix& adj, std::function<void(int&)> address = [](int& u)->void {std::cout << u; })
	{
		//访问过或者u不合法
		if (u<0||u>=vis.size()||vis[u])
		{
			return;
		}

		//标记已访问
		vis[u] = true;

		address(u);

		//递归搜索
		for (int i = 0; i < vis.size(); i++)
		{
			//存在邻接点
			if (adj.graph[u][i] != INT_MAX)
			{
				dfs(i, vis,adj,address);
			}
		}
	}
```

- 非递归

```cpp
//深度优先搜索（DFS）算法的非递归形式，类似于广度优先，但这里使用栈
	void dfs_non_recursive(int start, std::vector<bool>& vis, const Adj_Matrix& adj, std::function<void(int&)> address = [](int& u)->void {std::cout << u; })
	{
		//已经访问过或者start不合法
		if (vis[start] || start < 0 || start >= vis.size())return;

		std::vector<int> q;//存放当前连通分支节点

		q.push_back(start);//将起始节点入栈

		vis[start] = true;// 标记为已访问

		//栈不为空，即当前连通分支还有未访问的节点
		while (!q.empty())
		{
			int u = q.back(); // 获取栈顶的节点

			q.pop_back();           // 出栈

			address(u);       // 处理当前节点

			// 遍历当前顶点，找到所有邻接并且未访问的节点加入队列
			for (int i = 0; i < adj.graph.size(); i++)
			{
				if (adj.graph[u][i] != INT_MAX && !vis[i])
				{
					vis[i] = true;// 标记为已访问
					q.push_back(i);     // 将邻接节点入栈
				}
			}
			
		}
	}
```



- BFS:广度优先搜索

  - 非递归利用队列（类似树的层次遍历）
  - 可用于单源无权（权值为1）最短路

  ```cpp
  //广度优先搜索（BFS）算法（非递归）,并对节点进行处理,vis保存是否访问
  	void bfs(int start, std::vector<bool>& vis, const Adj_Matrix& adj, std::function<void(int&)> address = [](int& u)->void {std::cout << u; })
  	{
  		//已经访问过或者start不合法
  		if (vis[start] || start < 0 || start >= vis.size())return;
  
  		std::queue<int> q;//存放当前连通分支节点，并要着start节点一圈圈增加
  
  		vis[start] = true;//标记初始点访问
  
  		q.push(start);//将起始节点入队
  
  		//队列不为空，即当前连通分支还有为访问的节点
  		while (!q.empty())
  		{
  			int u = q.front(); // 获取队列前端的节点
  
  			q.pop();           // 出队
  
  			address(u);       // 处理当前节点
  
  			// 遍历当前顶点，找到所有邻接并且未访问的节点加入队列
  			for (int i=0;i<adj.graph.size();i++)
  			{
  				if (adj.graph[u][i] != INT_MAX && !vis[i])
  				{
  					vis[i] = true;// 标记为已访问
  					q.push(i);     // 将邻接节点入队
  				}
  			}
  		}
  	}
  ```

  

- **拓扑序列**：AOV网是一个有向无环图，可以用于证明图是否有环

  > 1. 选择一个入度为0的顶点并输出
  >
  > 2. 删除该顶点及该顶点引出的所有边
  >
  > 3. 执行①②，直至所有顶点已输出，或图中剩余顶点 入度均不为0（说明存在环，无法继续拓扑排序）
  > 4. 对于任何无环的AOV网，其顶点均可排成拓扑序列， 其拓扑序列**未必唯一**
  > 5. 拓展：**DFS可以输出拓扑序的逆序**
  >
  > ```cpp
  > std::vector<int> TopologicalSort(const Adj_Matrix& adj)
  > {
  >     // 如果是无向图，无法进行拓扑排序
  >     if (!adj.is_direct)
  >     {
  >         std::cerr << "Graph doesn't have direction, topological sorting not possible." << std::endl;
  >         return {};
  >     }
  > 
  >     int number = adj.graph.size();  // 获取图中节点数量
  > 
  >     std::vector<int> Topo;          // 存储拓扑排序结果
  >     std::queue<int> zero_in_degree; // 存储入度为0的节点
  > 
  >     // 存放各个节点的入度
  >     std::vector<int> indegree(number, 0);
  > 
  >     // 计算每个节点的入度
  >     for (int u = 0; u < number; u++)
  >     {
  >         for (int v = 0; v < number; v++)
  >         {
  >             // 如果存在边 u -> v，v的入度增加
  >             if (adj.graph[u][v] != INT_MAX)
  >             {
  >                 indegree[v]++;
  >             }
  >         }
  >     }
  > 
  >     // 将入度为0的节点放入队列
  >     for (int i = 0; i < number; i++)
  >     {
  >         if (indegree[i] == 0)
  >         {
  >             zero_in_degree.push(i);
  >         }
  >     }
  > 
  >     // Kahn算法：处理入度为0的节点
  >     while (!zero_in_degree.empty())
  >     {
  >         // 从队列中取出一个节点
  >         int u = zero_in_degree.front();
  >         zero_in_degree.pop();
  > 
  >         // 将该节点加入拓扑排序结果
  >         Topo.push_back(u);
  > 
  >         // 遍历该节点的所有邻接节点
  >         for (int i = 0; i < number; i++)
  >         {
  >             // 如果有边 u -> i，i的入度减一
  >             if (adj.graph[u][i] != INT_MAX)
  >             {
  >                 indegree[i]--;
  > 
  >                 // 如果i的入度为0，加入队列
  >                 if (indegree[i] == 0)
  >                 {
  >                     zero_in_degree.push(i);
  >                 }
  >             }
  >         }
  >     }
  > 
  >     // 检查是否存在环：如果拓扑排序结果的节点数不等于图的节点数，说明图中有环
  >     if (Topo.size() != number)
  >     {
  >         std::cerr << "Graph has a cycle, topological sorting not possible." << std::endl;
  >         return {};
  >     }
  > 
  >     // 返回拓扑排序结果
  >     return Topo;
  > }
  > 
  > ```
  >
  > 

- **关键路径**：完成整个工程所需的最短时间取决于从源点到汇点的最长路径长度

  > - 关键活动：活动的**最早开始时间等于活动 A 的最迟开始时间**， 即`l(i)＝e(i)`,也是不可以拖延的活动
  > - 关键路径：由关键活动组成的路径，亦即源点到汇点的最长路径，可能不止一条
  >
  > 1. 对AOE网求各顶点vj的最早发生时间ve(j)
  > 2. 求各顶点vj的最迟发生时间vl(j)；
  > 3. 求出各活动ai的最早开始时间e(i)和 最迟开始时间l(i)，若e(i)=l(i)，则ai是关键活动
  > 4. 具体算法
  >    1. 求出拓扑排序，若网中有环则终止算法，按拓扑序求出各顶点的最早发生时间ve
  >    2. 按逆拓扑序求各顶点的最迟发生时间vl
  >    3. 根据ve和vl的值，求各活动的最早开始时间e与最迟开始时间l，若`e=l`，则对应活动是关键活动，其中最晚开始时间和最早开始时间的差值为活动的**时间余量**。
  >    4. 因为拓扑序列不唯一，所以关键路径也不唯一。
  >
  > ```cpp
  > //关键路径不唯一
  > std::vector<int> CriticalPath(const Adj_Matrix& adj)
  > {
  >     // 检查是否为无向图
  >     if (!adj.is_direct)
  >     {
  >         std::cerr << "Graph doesn't have direction, CriticalPath not possible." << std::endl;
  >         return {};
  >     }
  > 
  >     int number = adj.graph.size();  // 获取图中节点数量
  > 
  >     // 获取拓扑排序
  >     std::vector<int> Topo = TopologicalSort(adj);
  > 
  >     // 如果拓扑排序为空，表示图中存在环，无法进行关键路径计算
  >     if (Topo.empty())
  >     {
  >         std::cout << "图中存在环，无法计算关键路径。" << std::endl;
  >         return {};
  >     }
  > 
  >     // 初始化边的数量
  >     int edge_num = 0;
  > 
  >     // 初始化每个节点的最早发生时间（VE），开始点的 VE 为0
  >     std::vector<int> VE(number, 0);
  > 
  >     // 计算每个节点的 VE
  >     for (int u = 0; u < Topo.size(); u++)
  >     {
  >         for (int v = 0; v < number; v++)
  >         {
  >             // 如果存在边 u -> v，更新 v 的 VE
  >             if (adj.graph[u][v] != INT_MAX)
  >             {
  >                 VE[v] = std::max(VE[v], VE[u] + adj.graph[u][v]);
  >                 edge_num++;  // 计算边的数量
  >             }
  >         }
  >     }
  > 
  >     // 初始化每个节点的最晚发生时间（VL），结束点的 VL 为 VE[number - 1]
  >     std::vector<int> VL(number, VE[number - 1]);
  > 
  >     // 逆拓扑排序计算每个节点的 VL
  >     for (auto it = Topo.rbegin(); it != Topo.rend(); it++)
  >     {
  >         int u = *it;
  >         for (int i = 0; i < number; i++)
  >         {
  >             if (adj.graph[u][i] != INT_MAX)
  >             {
  >                 VL[u] = std::min(VL[u], VL[i] - adj.graph[u][i]);
  >             }
  >         }
  >     }
  > 
  >     // 计算关键路径上的活动（弧的最早开始时间和最晚开始时间相同）
  >     std::vector<int> critical_adjpath;
  > 
  >     // 遍历拓扑排序中的每个节点，检查哪些弧是关键路径
  >     for (int u = 0; u < Topo.size(); u++)
  >     {
  >         for (int v = 0; v < number; v++)
  >         {
  >             // 如果存在边 u -> v，计算其最早开始时间 ET 和最晚开始时间 LT
  >             if (adj.graph[u][v] != INT_MAX)
  >             {
  >                 int ET = VE[u];  // 最早开始时间
  >                 int LT = VL[v] - adj.graph[u][v];  // 最晚开始时间
  > 
  >                 // 如果 ET == LT，则该弧是关键路径
  >                 if (ET == LT)
  >                 {
  >                     // 如果 critical_adjpath 为空，加入首尾节点
  >                     if (critical_adjpath.empty())
  >                     {
  >                         critical_adjpath.push_back(u);
  >                         critical_adjpath.push_back(v);
  >                     }
  >                     // 如果首尾节点相接，直接添加尾节点
  >                     else if (critical_adjpath.back() == u)
  >                     {
  >                         critical_adjpath.push_back(v);
  >                     }
  >                 }
  >             }
  >         }
  >     }
  > 
  >     // 输出项目的最早完成时间
  >     std::cout << "项目的最早完成时间为：" << VE[number - 1] << std::endl;
  > 
  >     // 返回关键路径
  >     return critical_adjpath;
  > }
  > 
  > ```
  >
  > 

- 最短路径
  - 无权图的单源最短路径问题：BFS
    > - BFS过程中，当访问某个顶点时，就确定了该点与源点的最 短距离
    > - 通过BFS，从源点开始由近及远求各顶点的最短路径v
    >
    > ```cpp
    > // 找到无权最短路径，图中所有边权值为1，求点v到其他各个点的最短路径和最短路径长度
    > // path[i] 记录从 v 到 i 的最短路径上顶点 i 的前驱结点
    > // dist[i] 记录从 v 到 i 的最短路径长度
    > void ShortestPath(const Adj_Matrix& adj, int v, std::vector<int>& dist, std::vector<int>& path)
    > {
    >     // dist 和 path 的初始化由调用方完成
    >     int number = dist.size(); // 获取图中顶点的数量
    > 
    >     // 创建一个队列用于广度优先搜索（BFS）
    >     std::queue<int> Q;
    >     Q.push(v); // 将起点 v 入队
    > 
    >     // 起点到自身的距离为0
    >     dist[v] = 0;
    > 
    >     // 求 v 到其他各个顶点的最短路径，类似于图的 BFS
    >     while (!Q.empty())
    >     {
    >         // 处理队头的顶点 u
    >         int u = Q.front();
    >         Q.pop();
    > 
    >         // 遍历当前点 u 的所有边（邻接节点）
    >         for (int i = 0; i < number; i++)
    >         {
    >             // 如果存在边 u -> i（即图中有连接）
    >             if (adj.graph[u][i] != INT_MAX)
    >             {
    >                 int k = i;  // 邻接点 k
    > 
    >                 // dist[k] == -1 表示未访问过该节点
    >                 if (dist[k] == -1)
    >                 {
    >                     // 将未访问的邻接点 k 入队
    >                     Q.push(k);
    > 
    >                     // 更新 dist[k] 为 u 到 k 的距离，等于 u 到起点的距离加 1
    >                     dist[k] = dist[u] + 1;
    > 
    >                     // 更新 k 的前驱节点为 u
    >                     path[k] = u;
    >                 }
    >             }
    >         }
    >     }
    > }
    > ```
    >
    > 
    
  - 正权图的单源最短路径问题：Dijkstra算法
    > - 找到各个局部最优路（任意最短路的前缀，也是一条最短路）
    > - 初始化起点到其他点距离
    > - 找局部最优路
    > - 从局部最优路更新到其他点的距离
    > - 重复直到所有点的最优路找到
    > - 可以利用优先队列（斐波那契堆）优化找局部最优路的步骤
    >
    > ```cpp
    > //利用优先队列维护最短路长度最小的结点，适用于稀疏图
    > 	void Dijkstra_ShortestPath_optimize(const Adj_Matrix& adj, int v, std::vector<bool>& vis, std::vector<int>& dist, std::vector<int>& path)
    > 	{
    > 		//创建优先队列，利用pair<T,int>分别存放距离，节点,默认T有greater
    > 		std::priority_queue<std::pair<int, int>, std::vector<std::pair<int, int>>, std::greater<std::pair<int, int>>> pq;
    > 
    > 		//初始化
    > 		dist[v] = 0;
    > 
    > 		//放入队列
    > 		pq.push({ 0,v });
    > 
    > 		//直到队列为空则完成
    > 		while (!pq.empty())
    > 		{
    > 			//取当前最短路长度最小的结点
    > 			std::pair<int, int> node = pq.top();
    > 			pq.pop();
    > 
    > 			//如果此点已经找到最小路径即局部最优路
    > 			int u = node.second;
    > 			if (vis[u])continue;
    > 
    > 			////如果有已经更新的最短路径,放弃这个记录
    > 			//if (node.first > dist[u])continue;
    > 			//此操作和上面判断相同
    > 
    > 			//标记
    > 			vis[u] = true;
    > 
    > 			//更新从此点出发的其他点最短路径
    > 			for(int i=0;i<adj.graph.size();i++)
    > 			{
    > 				//更小则更新
    > 				if (adj.graph[u][i] != INT_MAX && dist[u] + adj.graph[u][i] < dist[i])
    > 				{
    > 					//更新路径和前驱并放入队列
    > 					dist[i] = dist[u] + adj.graph[u][i];
    > 					path[i] = u;
    > 					pq.push({ dist[i] ,i });
    > 				}
    > 			}
    > 		}
    > 	}
    > ```
    >
    > 
    
  - 正权图的多源最短路径问题
    - 多次Dijkstra算法
    - Floyd算法（多用于邻接矩阵）
      
      > - 算法通过三重循环来更新最短路径。外层循环通过引入一个中间点 `k`，判断是否可以通过中间点 `k` 来缩短从 `i` 到 `j` 的路径。
      > - 如果通过 `k` 的路径更短，则更新 `dist[i][j]`，并且更新前驱节点 `path[i][j]` 为通过 `k` 到达 `j` 的前驱节点。
      >
      > ```cpp
      > void Floyd_ShortestPath(const Adj_Matrix& adj)
      > {
      >     // 将从Vi到Vj的最短路径长度初始化为邻接矩阵中的值
      >     std::vector<std::vector<int>> dist, path;
      > 
      >     // 初始化dist和path，大小与邻接矩阵相同
      >     dist.resize(adj.graph.size(), std::vector<int>(adj.graph.size(), 0));
      >     path.resize(adj.graph.size(), std::vector<int>(adj.graph.size(), -1));
      > 
      >     // 初始化dist和path
      >     for (int i = 0; i < adj.graph.size(); i++)
      >     {
      >         for (int j = 0; j < adj.graph.size(); j++)
      >         {
      >             dist[i][j] = adj.graph[i][j];
      > 
      >             // 如果i和j之间有边，则设置j的前驱为i
      >             if (dist[i][j] < INT_MAX)
      >                 path[i][j] = i; 
      >         }
      >     }
      > 
      >     // 使用三重循环来计算最短路径
      >     for (int k = 0; k < adj.graph.size(); k++)  // 中间点
      >     {
      >         for (int i = 0; i < adj.graph.size(); i++)  // 起点
      >         {
      >             if(i == k)continue;
      >             for (int j = 0; j < adj.graph.size(); j++)  // 终点
      >             {
      >                 if(j == k || j == i)continue;
      >                 // 如果通过k能得到更短的路径
      >                 if (dist[i][k] + dist[k][j] < dist[i][j])
      >                 {
      >                     // 更新最短路径长度
      >                     dist[i][j] = dist[i][k] + dist[k][j];
      > 
      >                     // 更新路径的前驱节点
      >                     path[i][j] = path[k][j];
      >                 }
      >             }
      >         }
      >     }
      > 
      >     // 打印结果（可以添加打印逻辑）
      > }
      > 
      > ```
      >
      > 
  
- 最小支撑树：边权之和最小的支撑树称为G的最小支撑树

  -  Prim算法（加点法）
    
    > - 选择任一点u做为起点，放入集合S，即令S={u}(u属于V)；
    > - 找最小跨集合边(u, v) ，即端点分别属于集合S和V-S且权值 最小的边，将该边加入最小支撑树，并将点v放入S；
    > - 执行②，直至S=V
    >
    > ```cpp
    > // 普里姆算法优化，使用优先队列
    > Adj_Matrix MiniSpanTree_Prim(const Adj_Matrix& adj, int u = 0 /*起始点*/) {
    >     // 非连通图，返回空图
    >     if (Connected_Component(adj) != 1) {
    >         return Adj_Matrix(0);
    >     }
    > 
    >     int n = adj.graph.size();  // 图的顶点数
    >     Adj_Matrix MiniSpanTree(n, adj.is_direct);  // 最小生成树
    > 
    >     // 记录顶点是否已经加入生成树
    >     std::vector<bool> vis(n, false);
    > 
    >     // 使用优先队列（最小堆）保存未加入生成树的点和其对应的最小边权值
    >     // 队列中存储的是 (边权值, 顶点) 的 pair
    >     std::priority_queue<std::pair<int, int>, std::vector<std::pair<int, int>>, std::greater<>> pq;
    > 
    >     // 初始化：从起始点u开始，加入队列，权值为0
    >     pq.push({0, u});
    > 
    >     // 选择其他n-1个顶点，生成n-1条边
    >     while (!pq.empty()) {
    >         // 取出当前权值最小的边
    >         int current_weight = pq.top().first;
    >         int u0 = pq.top().second;
    >         pq.pop();
    > 
    >         // 如果顶点u0已经加入生成树，则跳过
    >         if (vis[u0]) continue;
    > 
    >         // 标记u0为已访问
    >         vis[u0] = true;
    > 
    >         // 更新最小生成树的边
    >         if (u0 != u) {  // 排除起始点
    >             int v0 = pq.top().second;  // 顶点u0的前驱
    >             MiniSpanTree.graph[u0][v0] = current_weight;
    > 
    >             // 无向图则增加对称边
    >             if (!MiniSpanTree.is_direct) {
    >                 MiniSpanTree.graph[v0][u0] = current_weight;
    >             }
    >         }
    > 
    >         // 更新与u0的相邻节点的最小边，并加入优先队列
    >         for (int i = 0; i < n; i++) {
    >             if (!vis[i] && adj.graph[u0][i] < INT_MAX) {  // 如果i未访问且有边
    >                 pq.push({adj.graph[u0][i], i});
    >             }
    >         }
    >     }
    > 
    >     // 返回生成的最小生成树
    >     return MiniSpanTree;
    > }
    > ```
    >
    > 
  - Kruskal算法（逐边加入）所以不针对邻接矩阵为例
    > - 在G中选择权值最小的边，并将此边从G中删除
    > - 若该边加入T后不产生环（即此边的两个端点在T的不同连 通分量中），则将此边加入T中，从而使T减少一个连通分 量，否则本步骤无操作，对于是否产生环可以利用并查集
    > - 重复①②直至T中仅剩一个连通分量
    >
    > ```cpp
    > //克鲁斯卡尔 (Kruskal)算法，可称为“加边法”，适用于稀疏图
    > 	//每次选出权值最小并且无法使现有的树形成环的边加入最小支撑树,返回一个图
    > 	std::vector<Edge> MiniSpanTree_Kruskal(std::vector<Edge> graph,int number)
    > 	{
    > 		//非连通图
    > 		if (Connected_Component(graph,number) != 1)
    > 		{
    > 			return{};
    > 		}
    > 		std::vector<Edge> MiniSpanTree;
    > 		//在Edge增加了weight成员存储权值，可以直接用sort排序
    > 		std::sort(graph.begin(), graph.end(), [](const Edge& a, const Edge& b)->bool {return a.weight < b.weight; });
    > 
    > 		//辅助数组Vexset,标识各个顶点所属的连通分量,类似于并查集
    > 		std::vector<int> Vexset;
    > 		Vexset.resize(number,0);
    > 		//初始化,表示各顶点自成一个连通分址
    > 		for (int i = 0; i < number; i++)
    > 		{
    > 			Vexset[i] = i;
    > 		}
    > 
    > 		//开始创建最小支撑树
    > 		for (int i = 0; i < graph.size(); i++)
    > 		{
    > 			int v1 = graph[i].u;
    > 			int v2 = graph[i].v;
    > 			int vs1 = Vexset[v1];
    > 			int vs2 = Vexset[v2];
    > 
    > 			//边的两个顶点不在同一连通分量
    > 			if (vs1 != vs2)
    > 			{
    > 				//加入此边
    > 				MiniSpanTree.push_back(Edge(v1, v2));
    > 
    > 				//合并vs1和vs2两个分量，即两个集合统一编号
    > 				for (int j = 0; j < number; j++)
    > 				{
    > 					if (Vexset[j] == vs2)Vexset[j] = vs1;
    > 				}
    > 			}
    > 		}
    > 
    > 		//返回
    > 		return MiniSpanTree;
    > 	}
    > ```
    >
    > 
  
  

# 排序

## 定义

排序(Sorting)是按**关键字**的非递减或非递增顺序对一组记录重新进行排列的操作

排序的稳定性：关键字相同的记录排序前后的相对位置不变

## 内排序

内部排序的过程是一个逐步扩大记录的有序序列长度的过程。在排序的过程中，可以将排序记录区分为两个区域：有序序列区和无序序列区。 

使有序区中记录的数目增加一个或几个的操作称为一趟排序。

### 插入排序

每一趟将一个待排序的记录，按其关键字的大小插入到已经排好序的一组记录的适当位置上，直到所有待排序记录全部插入为止

- **插入排序**

> 1. 直接插入排序：将一条记录插入到已排好序的有序表中，从而得到一个新的、 记录数量增1的有序表。
>
>    ```cpp
>    //直接插人排序，O(n^2)
>    //稳定排序,更适合于初始记录基本有序（正序）的情况
>    //也适用千链式存储结构，只是在单链表上无需移动记录，只需修改相应的指针
>    template<class T=int>
>    void Straight_Insertion_Sort(T a[], int n)
>    {
>    	//对顺序表L做直接插入排序
>    	//数组从0开始，第零个元素已经有序,所以从1开始排序
>    	for (int i = 1; i < n; i++)
>    	{
>    		//记录要插入的元素
>    		T key = a[i];
>    		   
>    		//从i-1位置往前找位置,同时后移元素
>    		int j = i - 1;
>    		while (j >= 0 && key < a[j])
>    		{
>    			//后移
>    			a[j + 1] = a[j];
>    			j--;
>    		}
>       
>    		//插入
>    		a[j + 1] = key;
>    	}
>    }
>    ```
>
>    2. 折半插入排序：在直接插入排序的基础上优化"查找"即找到插入位置，，这个 “查找＂ 操作可利用 “**折半查找**” 来实现
>
>    ```cpp
>    //折半插人排序，O(n^2)
>    //在已经排序的有序数组里采用二分查找，提高找到插入位置的效率
>    //稳定排序,适合初始记录无序、n较大时的情况。
>    //只能用于顺序结构
>    template<class T = int>
>    void Binary_Insertion_Sort(T a[], int n)
>    {
>    	//对顺序表L做折半插入排序
>    	for (int i = 1; i < n; i++)
>    	{
>    		//记录要插入的元素
>    		T key = a[i];
>       
>    		//二分查找位置,在[0,i-1]找
>    		int low = 0;
>    		int high = i - 1;
>    		while (low <= high)
>    		{
>    			//折半
>    			int mid = (low + high) / 2;
>    			//更新搜索区间
>    			if (key < a[mid])high = mid - 1;
>    			else low = mid + 1;
>    		}
>       
>    		//找到插入位置，为high+1(/low)
>    		   
>    		//后移元素,high+1(/low)
>    		for (int j = i - 1; j >= high + 1; j--)a[j + 1] = a[j];
>       
>    		//插入
>    		a[high + 1] = key;
>    	}
>    }
>    ```
>

- **希尔排序（缩小增量排序）**

采用**分组插入**的方法。先将整个待排序记录序列分割成几组，从而减少参与直接插入排序的数据量，对每组分别进行直接插入排序，然后增加每组的数据量，重新分组。 这样 当经过几次分组排序后，整个序列中的记录“基本有序” 时，再对全体记录进行一次直接插入排序。

希尔对记录的分组，不是简单地 ”逐段分割＂，而是将相隔某个 **“增量”** 的记录分成一组。

具体步骤

> //将待排序序列分为若干子序列（每个子序列的元素在原始数组中间距相同）
> //对这些子序列进行插入排序
> //减小每个子序列中元素之间的间距，重复上述过程直至间距减少为1。

```cpp
//记录跳跃式地移动导致排序方法是不稳定的，只能用于顺序结构
//n越大时，效果越明显。所以适合初始记录无序、n较大时的情况
template<class T>
void ShellSort(T a[], int n)
{
	//初始化间隔 h，使用 Knuth 序列计算使其小于数组长度的最大值
	int h = 1;

	//生成最大增量
	while (h < n / 3)
	{
		h = 3 * h + 1;
	}

	//进行希尔排序，逐渐减少间隔 h，直到 h 减小到 1（最后一次遍历）
	while (h >= 1)
	{
		//对每一个间隔为 h 的子数组进行插入排序
		for (int i = h; i < n; i++)
		{
			//将 a[i] 插入到其对应的子数组中的正确位置
			for (int j = i; j >= h && a[i] < a[j - h]; j -= h)
			{
				std::swap(a[j], a[j - h]);//类似后移
			}
		}
		// 缩小间隔，使 h 逐渐减小，最终变为 1
		h = h / 3;
	}
}

```

- 可以提前生成增量序列

```cpp
template<class T>
void ShellSort_C(T a[], int n,int t,int dk[])
{
	//dk[]存放着生成好的增量序列
	//有多种增量序列
	//希尔增量序列（2^k - 1）
	//Hibbard增量序列（1, 3, 7, 15, ...）
	//Sedgewick增量序列（1, 5, 19, 41, ...）

	for (int i = 0; i < t; i++)
	{
		Shellinsert_C(a, n, a[i]);
	}
}

//C语言版
template<class T>
void Shellinsert_C(T a[], int n,int dk)
{
	int d = dk;//此次增量
	//插入排序
	for (int i = d; i < n; i++)
	{
		int j;
		if (a[i] < a[i - d])
		{
			//存在无序
			int key = a[i];

			//插入
			for (j = i - d; j >= 0 && key < a[j]; j -= d)
			{
				a[j + d] = a[j];
			}

			a[j + d] = key;
		}
	}
}
```

### 交换排序



- 选择排序
- 堆排序
- 分布排序
  - 基数排序
  - 计数排序
  - 桶排序
- 堆排序



# 查找

- 顺序查找
- 对半查找
- 斐波那契查找
- 插值查找
- 分块查找

