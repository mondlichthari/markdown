使用 vector 前，需要包含头文件：
#include<vector>

创建 vector
创建一个空 vector：
std::vector<int>vec;
即vector<数据类型>数组名称；

#**动态：**

使用 push_back() 向尾部添加元素：
vec.push_back(100);

pop_back() 在尾部删除元素，（）内不需要写内容

vec.size()访问数组长度
vec.capacity()检查容量
size：当前元素数量。
capacity：当前已分配的内存容量。

vec[]访问数组元素，和普通数组一样
vec.at()会检查是否越界，安全

修改某个元素的值，例如vec[2]=3,和普通数组一样

清空所有元素且释放内存，用vector<数据类型>().swap(数组名称)，
例如vector<int>().swap(vec)

#**静态：**
创建一个空 vector：
std::vector<int>vec;

指定初始大小：
std::vector<int>vec(5);
以上代码会创建 5 个元素，默认值为 0。

指定初始值：
std::vector<int>vec(5, 10);

创建结果：
[10, 10, 10, 10, 10]

使用初始化列表：
std::vector<int>vec = {1, 2, 3, 4};
