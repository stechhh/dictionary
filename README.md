# dictionary
Python中关于字典的基础知识

# 什么是字典？
字典,是一系列键值对。每个键都与一个值相关联，你可使用键来访问相关联的值。与键相关联的值可以是数、字符串、列表乃至字典。字典用放在花括号（{}）中的一系列键值对表示。
键值对：是两个相关联的值。

# 基础知识
## 使用字典 
### 访问字典中的值：
![image](https://user-images.githubusercontent.com/130123927/234269181-883fd50b-fcd8-4f27-999e-7705e26e3ab2.png)
   制定的键不存在时会引发问题。 

案例：
```python
alien_0 = {'color': 'green'}
print(alien_0['color'])
```

### 添加键值对
![image](https://user-images.githubusercontent.com/130123927/234268992-c25418f0-8397-4e4f-88e6-1d652c6913ab.png)

案例：
```python
alien_0 = {'color':'green', 'points':5}
print(alien_0)

alien_0['x_position'] = 0
alien_0['y_position'] = 25
print(alien_0)
```
