# dictionary
Python中关于字典的基础知识

# 什么是字典？
字典,是一系列键值对。每个键都与一个值相关联，你可使用键来访问相关联的值。与键相关联的值可以是数、字符串、列表乃至字典。字典用放在花括号（{}）中的一系列键值对表示。
键值对：是两个相关联的值。

# 基础知识
## 访问字典中的值：
![image](https://user-images.githubusercontent.com/130123927/234269181-883fd50b-fcd8-4f27-999e-7705e26e3ab2.png)
   制定的键不存在时会引发问题。 

案例：
```python
#输出键'color'的值
alien_0 = {'color': 'green'}
print(alien_0['color'])
```

### 添加键值对
![image](https://user-images.githubusercontent.com/130123927/234268992-c25418f0-8397-4e4f-88e6-1d652c6913ab.png)

案例：
```python
#创建并输出字典
alien_0 = {'color':'green', 'points':5}
print(alien_0)

#添加两个键值对并输出字典
alien_0['x_position'] = 0
alien_0['y_position'] = 25
print(alien_0)
```

## 先创建一个空字典
![image](https://user-images.githubusercontent.com/130123927/234272846-d4bcee59-56f9-4124-a308-755edb22c67e.png)

使用字典来存储用户提供的数据或在编写能自动生成大量键值对的代码时，通常需要先定义一个空典。

案例：
```python
#创建一个空字典
alien_0 = {}

#添加键值对
alien_0['color'] = 'green'
alien_0['points'] = 5

print(alien_0)
```

## 修改字典中的值
![image](https://user-images.githubusercontent.com/130123927/234273565-f4327c39-1c27-4b06-ad7a-f189aa7a4e8f.png)

案例：
```python
#创建并输出字典
alien_0 = {'color':'green'}
print(f"The alien is {alien_0['color']}.")

#修改键'color'的值，并输出字典
alien_0['color'] = 'yellow'
print(f"The alien is now {alien_0['color']}.")
```

## 删除键值对
![image](https://user-images.githubusercontent.com/130123927/234275711-37912b0f-b169-4a9f-bf00-a5d54f38f645.png)

删除的键值对会永远消失

案例：
```python
#创建并输出字典
alien_0 = {'color':'green', 'points':5}
print(alien_0)

#删除键'points'及其值并输出字典
del alien_0['points']
print(alien_0)
```

## 由类似对象组成的字典
确定需要使用多行来定义字典时，要在输入 左花括号后按回车键。在下一行缩进四个空格，指定第一个键值对，并在它后面加上一个逗号。此后再按回车键时，文本编辑器将自动缩进后续键值对，且缩进量与第一个键值对相同。

案例：
```python
#创建字典
favorite_languages = {
    'jen': 'python',
    'sarah': 'c',
    'edward': 'ruby',
    'phil': 'python',
    }
 
#输出sarah最喜欢的语言
language = favorite_languages['sarah'].title()
print(f"Sarah's favorite language is {language}.")
```

## 使用get()来访问值
第一个参数用于指定键，是必不可少的；第二个参数为指定的键不存在时要返回的值。

注：调用get()时，如果没有指定第二个参数且指定的键不存在，Python将返回值None。

案例：
```python
#创建字典
alien_0 = {'color':'green', 'speed':'slow'}

#获取与键'points'相关的值,若不存在返回No point value assigned.
point_value = alien_0.get('points', 'No point value assigned.')
print(point_value)
```












