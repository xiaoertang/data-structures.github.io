# 线性表——顺序表

###### 顺序表示指的是用一组地址连续的存储单元依次存储线性表的数据元素，这种表示 也称作线性表的顺序存储结构或顺序映像。通常，称这种存储结构的线性表为顺序表(Sequenital List)。其特点是，逻辑上相邻的数据元素，其物理次序也是相邻的。 

一般来说， 线性表的第l个数据元素ai的存储位置为： LOC(ai = LOC(a1) + (i - 1) x l 

### 一、//－－－－－顺序表的存储结构－－－－－

#define MAXSIZE 100         //顺序表可能达到的最大长度

 typedef struct 

｛    ElemType *elem;     //存储空间的基地址

​       int length;                  // 当前长度

 }SqList;                          //顺序表的结构类型为SqList


### 二、顺序表中基本操作的实现 

##### 1.初始化 

![1](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV07RAmEaNuFUD.3c7TA3ZCg0nDAMqUcJGrE6X77hkofhW7eICcjBztP3.Ik0fiVIKZQ!!/c&ek=1&kp=1&pt=0&bo=FwSnAQAAAAARF5U!&t=5&tl=3&vuin=1298840110&tm=1592038800&sce=60-2-2&rf=newphoto&t=5)

动态分配线性表的存储区域可以更有效地利用系统的资源， 当不需要该线性表时 ， 可以使用 销毁操作及时释放占用的存储空间。 

##### 2.取值

![1](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV07RAmEaNuFUD.3c7TA3ZCg0nDAMqUcJGrE6X77hkofhW7eICcjBztP3.Ik0fiVIKZQ!!/c&ek=1&kp=1&pt=0&bo=FwSnAQAAAAARF5U!&tl=3&vuin=1298840110&tm=1592038800&sce=60-2-2&rf=0-0)

##### 3.查找

![3](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV0wOLjLQnMqrf1tp9GkR1wO93dT1UBRqNBnmWQzJzWkyO4582eET3.sZrAWqRR6884Q!!/c&ek=1&kp=1&pt=0&bo=oAQTAgAAAAARF5U!&tl=3&vuin=1298840110&tm=1592042400&sce=60-2-2&rf=0-0)

###### 顺序表的查找时间复杂度为O(n)

##### 4.插入

![4](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV0w*aPX6tUhdoCOTm2.1VL0wI8jkRW1XQUSI5UG0p04GeyoYYKS7JUPgYIg74lGQJJQ!!/c&ek=1&kp=1&pt=0&bo=ewT0AQAAAAARF6o!&tl=3&vuin=1298840110&tm=1592042400&sce=60-2-2&rf=0-0)



##### 顺序表插入算法的平均时间复杂度为O(n)，插入需要移动n-i+1个元素

##### 5.删除

![6](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV02W7JHfeGqd4v5qQespZaSMkl8iT.aDSfQI.sZLpjcABXEnbh2tNxkSwhGisENXW7A!!/c&ek=1&kp=1&pt=0&bo=LgTCAAAAAAARF8g!&tl=3&vuin=1298840110&tm=1592118000&sce=60-2-2&rf=0-0)

![7](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV06nkW7aOqG5CJHMySIJANRDM2ZVfCWL5MpZexKJRLZddcOhni.ubNpcoVv.u75OEtg!!/c&ek=1&kp=1&pt=0&bo=1QMZAQAAAAARF.4!&tl=3&vuin=1298840110&tm=1592118000&sce=60-2-2&rf=0-0)

##### 顺序表删除算法的平均时间复杂度为O(n)，插入需要移动n-i个元素

### [目录](https://github.com/xiaoertang/data-structures.github.io/blob/master/catalog/catalog.md)

### 上一节：[基本概念和术语](https://github.com/xiaoertang/data-structures.github.io/blob/master/1-introduction/introduction.md)

### 下一节：[单链表](https://github.com/xiaoertang/data-structures.github.io/blob/master/2-linear-list/2-linked-list.md)

