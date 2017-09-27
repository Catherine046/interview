# python元组、字典、列表

## 元组(tuple)：
###元组常用小括号表示，即：()，元素加逗号，是元组的标识，**不可修改**。

```python
    tuple = ('a','b','c','d') 
    #使用for循环进行遍历元组
    for each in tuple:
        print each
    #通过range()函数和for循环获取元组内元素的序号
    for index in range(len(tuple)): 
        print tuple[index]
```
###转换
- 元组转为字符串，print tup.__str__()
- 元组转为列表，print list(tup)
- 元组不可以转为字典


## 列表(list):
###列表常用方括号表示，即：[]，列表是**可变**的数据类型，即这种类型是可以被改变的，并且列表是可以嵌套的。

```python
    list = ['a','b','c','d']
    for each in list
        print(each,len(each))
    #通过range()函数和for循环获取元组内元素的序号
    for i in range(len(list)): 
        print list[i]
```
###列表中常用的函数：
 - cmp(list1,list2)：比较两个列表的元素 　　
 - len(list)：返回列表元素个数
 - max(list)：返回列表元素最大值 　
 - min(list)：返回列表元素最小值 　　
 - list(tuple)：将元组转换为列表

###列表中常用的9个方法：

 - list.append(obj)：在列表的末尾添加新的对象 　　
 - list.count(obj)：统计某个元素在列表中出现的次数
 - list.extend(list)：在列表末尾添加包含多个值的另一个序列，有扩展列表的作用
 - list.insert(index,obj)：将对象插入列表中的第index元素之前
 - list.pop(obj=list[-1])：默认移除列表中的一个元素（默认最后一个元素），并且返回该元素的值 
 - list.remove(obj)：移除列表中某个值 　　
 - list.reverse()：将列表中的元素反向排列
 - list.sort(function())：将列表进行排序
###转换
- 列表转为字符串，print str(nums)
- 列表转为元组，print tuple(nums)
- 列表不可以转为字典

##字典(dict)
###字典是由花括号{}来包含其数据的，花括号内包含键(key)和其对应的值(value)，key是唯一的。访问字典：由于字典是无序的，访问字典不能通过索引的方式；通过变量名[键名]来访问。字典添加项：变量名:[新添加的键名] = 新添加的键对应的值。字典修改项的值:变量名:[要修改的键名] = 新值
```python
    dict = {'name':'john','age':20,'sex':male}
    dict['class']='一班'   #添加班级
    for key,value in dict.items():
        print key,value
    结果：
    name john
    age 20
    sex male
    class 一班
```

###常用方法和操作：

1. D.get(key, defualtValue)：获得key对应的值，若key不存在，则返回设置的默认值defualtValue,若没有设置默认值则返回None。
2. D.has_key(key) ：检查字典中是否存在键key，有该键返回TRUE，否则FALSE。
3. D.keys()：返回由字典所有键构成的列表。 
4. D.values()：返回由字典所有值构成的列表。
5. D.items()：返回由字典所有键值对构成的列表，即[(key1,value1),(key2,value2),(key3,value3),...]
6. D.update(dic2)：将字典dic2中的元素合并到字典D中。
7. D.popitem()：随机删除字典中的一个键值对（一项），并返回值。若字典为空则抛出异常。
8. D.clear()：清空字典中的元素并返回None
9. D.pop(key)：删除指定键所对应的项，并返回key对应的值。key不能为空，也不默认删除排在最后的元素，因为字典是无序的，注意和列表的区别！！！
10. D.copy()：拷贝字典，两个字典不是同一个字典。如d = {1:1,2:2},d1 = d.copy() ->d1 = {1:1,2:2}。
11. cmp(dict1,dict2)：比较字典，(优先级为元素个数、键大小、键值大小)，第一个大则返回1，第一个小则返回-1，一样大则返回0。

###转换
- 字典转为字符串，print type(str(dict)), str(dict)
- 字典转化为元组：print tuple(dict)
- 字典转为列表，print list(dict)

