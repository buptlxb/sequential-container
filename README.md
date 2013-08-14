# sequential-container

C++ Primer Chapter 9 Sequential Container
今天又看了一遍顺序容器，因为总是很多东西看完不用就忘记了。希望在这里总结一下，作为对自己的检验和提醒，如果不小心也帮到了你的忙，我会更高兴。

### 顺序容器的定义
这里主要说三个顺序容器：
- vector：支持快速随机访问
- list：支持快速插入／删除
- deque：双端队列

=
##### 顺序容器的定义
为了使用这三个顺序容器，必须先包含相关的头文件，即下列文件：
```c++
#include <vector>
#include <list>
#include <deque>
```
vector，list，deque都是模版类，要定义某种特殊的容器，必须在容器名后加一对尖括号，尖括号里面提供容器中存放的元素的类型：
```c++
vector<string> svec; //empty vector that can hold strings
list<int> ilist; //empty list than can hold ints
deque< vector<string> > svdeq; //empty deque that can hold vector<string>s
```
=
##### 容器元素的初始化
