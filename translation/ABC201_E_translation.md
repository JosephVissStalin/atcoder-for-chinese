## 题意

有一棵 $N$ 个点，带边权的树。

对于点对 $(x,y)$，定义 $dist(x,y)$ 为 $x$ 到 $y$ 最短路上的所有边边权的异或和。

求出 $(\sum_{i=1}^ N \sum_{j=i+1} ^ N dist(i,j))\bmod (10^9+7)$。

## 数据范围 

$2\le N\le 2\times 10^5$。

$1\le u_i < v_i \le N$。

树的边权为 $w_i$，$0\le w_i < 2^{60}$。

输入的都是整数。

## 输入格式

第一行一个整数 $N$。

接下来 $N-1$ 行，每行三个整数 $u_i,v_i,w_i$。

## 输出格式

输出 $(\sum_{i=1}^ N \sum_{j=i+1} ^ N dist(i,j))\bmod (10^9+7)$。

## 样例

### 样例输入 1

```
3
1 2 1
1 3 3
```

### 样例输出 1

```
6
```



### 样例输入 2

```
5
3 5 2
2 3 2
1 5 1
4 5 13
```

### 样例输出 2

```
62
```



### 样例输入 3

```
10
5 7 459221860242673109
6 8 248001948488076933
3 5 371922579800289138
2 5 773108338386747788
6 10 181747352791505823
1 3 803225386673329326
7 8 139939802736535485
9 10 657980865814127926
2 4 146378247587539124
```

### 样例输出 3

```
241240228
```



## 样例解释

对于样例 1，$dist(1,2)=1,dist(1,3)=3,dist(2,3)=2$。

对于样例 3，**记得 $\bmod (1e^9+7)$。**

