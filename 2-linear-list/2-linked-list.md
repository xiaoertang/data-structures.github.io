# 线性表——单链表

### 线性表链式存储结构的特点是：用一组任意的存储单元存储线性表的数据元素（这组存储单 元可以是连续的，也可以是不连续的）。 单链表是一个结点，结点由两域组成，即其中存储数据元素信息的域称为数据域；存储直接后继存储位置的域称 为指针域。

### 链表中第一个结点的存储位置叫做头指针

### 单链表的第一个结点前附设一个结点，称为头结点

![1](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV070Id1Ycd8*EDFh82tqx6t7CBipRdJ*pkLrJVqzdxvGxXz1B0FXgbUgrREFhMXgOgQ!!/c&ek=1&kp=1&pt=0&bo=dgJjAQAAAAARFzY!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

### 一、单链表的存储结构

![1](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV02Lm*zOmcwnndlBuMNLBygNqaH0jxMDi8cqy2EVXFA2D2k085*URygNULIp.YorZPQ!!/c&ek=1&kp=1&pt=0&bo=wwJsAAAAAAARF40!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

### ![2](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV07pd1GbSuuMI4UGGnZs.D4HQRtD2NCJN3Hcw5f3p5cpgYTGlOXXA*GPCl6v7CqwRiA!!/c&ek=1&kp=1&pt=0&bo=uwNWAAAAAAARF84!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

### 二、单链表基本操作的实现

##### 1.初始化

单链表的初始化操作就是构造一个空表

![3](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV035Vuq0cWxqPvoeYMa*Zk1gRMi2s*bx*7AymARQUWlPuWIIJrvBdoF4GXIJ3VcgH4A!!/c&ek=1&kp=1&pt=0&bo=pwNrAQAAAAARF.4!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

##### 2.取值

和顺序表不同，链表中逻辑相邻的结点并没有存储在物理相邻的单元中，这样， 根据给定的 结点位置序号i'在链表中获取该结点的值不能像顺序表那样随机访问，而只能从链表的首元结 点出发，顺着链域next逐个结点向下访问。 

![4](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV0.G*MMzvFG1zXMjhrfcR0PaT90WTsefCSI.ZQsQSd9RuUNPKS.hm*5ZYyvSAGRAQfw!!/c&ek=1&kp=1&pt=0&bo=JATxAAAAAAARF*E!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)



![5](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV03FgfMY9oDQJgWw55RV6pDKYo1yuvxUl3jxist0LucnUtiW0UDMZ6bo6PkPlPRJp3g!!/c&ek=1&kp=1&pt=0&bo=QQRLAgAAAAARFyw!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

##### 单链表取值算法的平均时间复杂度为O(n)。

##### 3.查找

链表中按值查找的过程和顺序表类似，从链表的首元结点出发，依次将结点值和给定值e进 行比较，返回查找结果。 

![7](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV08*g0RVvk.TjCMgHZdpAS.CkR5v9q5MQq4JXgGxMhLeTY1aI8iwSC8NimU7mU0SuUA!!/c&ek=1&kp=1&pt=0&bo=TgRsAQAAAAARFwc!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

![8](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV00C3CT9VOK5RNN1fqzOCUt5qGes*ZuqLCs6DR578eyWw5HwoUJHOhynkgcKa0TgWgw!!/c&ek=1&kp=1&pt=0&bo=1gOhAAAAAAARF1Q!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

##### 4.插入

![14](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV06QWBTtCPnNmfWGo616nb1*Nhedwn7c7xPxYpW2czX6cSpD4mnM19DweKahiYj2dbw!!/c&ek=1&kp=1&pt=0&bo=UAQXAgAAAAARF2E!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

![9](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV01oJYa5md7RSLSZpPLF4WnQgJ2uf4PaDfiILVgn0i0Dsk3nbr4r5QcxX1ZwQsZI.XQ!!/c&ek=1&kp=1&pt=0&bo=RgS8AgAAAAARF9w!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

![11](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV0w8oPW8la6tflLXnmFl*cSgmN9HPqy8LpuzjmPEaRGF00zl.sgDEjAkR0b50LToj7A!!/c&ek=1&kp=1&pt=0&bo=PANoAAAAAAARF3c!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

##### 5.删除

![15](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV09xutxPCujCGukNzAMMZDtVyvnqL953SuAi5HvDZeOG8zC6rSePlDEf5Z4Q5MD7U6g!!/c&ek=1&kp=1&pt=0&bo=PAQWAQAAAAARFw8!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

![12](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV06X2SoJg*fvR5cvq6fWm1zJ*R.gTvMTNw5.RkIMLjgFvUM0BoRQwaFSGJqkfOljVgg!!/c&ek=1&kp=1&pt=0&bo=9APNAQAAAAARFxs!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

![13](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV0xYZXV3mehfOflhNBT1Db9BGsfq*YvfQZIg1jMsuo*flhL9JCYiby0q2*HFJULdQLg!!/c&ek=1&kp=1&pt=0&bo=mAPgAAAAAAARF1s!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

##### 6.单链表整表创建

###### （1）前插法创建单链表

![16](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV06p*L0D7hFhi9moX1RNHc**9PDn9Y22lHxY7AN1KXbRvrlCsVlNjIzW1tzBUraXKDg!!/c&ek=1&kp=1&pt=0&bo=zgLuAAAAAAARFwI!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

![17](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV0.Sp.VCGQ5BoPh2GWXo833mDz*sXFeiqSaWc3IGzzI*w6EkbRXV0HAGHgduJSSpF2A!!/c&ek=1&kp=1&pt=0&bo=NgN0AQAAAAARF2A!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

###### （2）后插法创建单链表

![178](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV0yR6UBAK7A6xXCF1h7PeYrGWw8umpaoYWYUxIPkQZPhI5d6AqAn.H2i5tptUio4HAg!!/c&ek=1&kp=1&pt=0&bo=0AI2AQAAAAARF8U!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

![112](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV06JKOQAKwERnzIlvOp26vDiMKVrAAGR0CUtc7XzDMd7lkPg71yfKI9EXhAuJsrJbSQ!!/c&ek=1&kp=1&pt=0&bo=IwPcAQAAAAARF90!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

### 三、单链表结构与顺序表结构优缺点

![113](http://a1.qpic.cn/psc?/V13qV41h2syAL4/zfrllz9Q9AzvUwq**DIV0zmfiu1Epq5SiqG8Ai5TLXlDaEEaKp6XaYt49BAAiwFYLmk5P.J.Ib*EUqnom*7CwA!!/c&ek=1&kp=1&pt=0&bo=ZAOOAQAAAAARF8g!&tl=3&vuin=1298840110&tm=1592121600&sce=60-2-2&rf=0-0)

### [目录]((https://github.com/xiaoertang/data-structures.github.io/blob/master/catalog/catalog.md)

### 上一节：[顺序表](https://github.com/xiaoertang/data-structures.github.io/blob/master/2-linear-list/1-sequence-list.md)

### 下一节：[双向链表]((https://github.com/xiaoertang/data-structures.github.io/blob/master/2-linear-list/3-double-linked-list.md)

