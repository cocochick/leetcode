# stl容器
## 通用函数
逆转
```cpp
#include<algorithm>
void reverse(vec.begin(),vec.end());    //或void reverse(vec,int begin,int end);
```
设置容器大小

    resize()    //实际分配内存


设置容器容量

    reserve()   //并未实际分配内存


## vector 向量

```cpp
pop_back(); //删除最后一个元素
erase(iterator pos);    //删除指定位置的元素，返回该元素下一个位置的迭代器
erase(beg,end); //删除位于迭代器[beg,end)位置的元素，返回end处迭代器
remove();   //删除容器中所有和指定元素值相等的元素，返回指向最后一个元素后的迭代器
clear();    //删除所有元素
```
## stack 栈

## queue 队列

## string 字符串

## priority_queue 优先队列
优先队列中，元素被赋予优先级，遵守最高级先出的特征，其本质是使用堆实现的。  
定义：priority_queue<Type, Container, Functional>  
Type为数据类型，Container为存储容器（STL中默认使用vector），Functional为比较方式（默认为less，即大顶堆）  
例如：
```cpp
//升序队列，小顶堆
priority_queue <int,vector<int>,greater<int> > q;
//降序队列，大顶堆
priority_queue <int,vector<int>,less<int> > q;
```

## deque 双向队列

## set 集合

## multiset 有序多重集合

## map 映射容器
