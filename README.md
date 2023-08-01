# Python-18-
Python学习笔记(18)
# p59 字典的实现原理
#通过hash函数来找value，因此查找效率是非常快的



# p60 字典的创建
#1.y\也是最常用的，使用{}
scores={'张三':100,'李四':98,'王五':45}
print(scores)
print(type(scores))

#2.使用内置函数dict()
student=dict(name='jack',age=20)  #这里的是否使用单引号取决于赋值的类型，此例前面为字符串，因此要加引号
print(student)

'''空字典'''
d={}
print(d)



# p61 字典元素的获取
scores={'张三':100,'李四':98,'王五':45}
'''第一种方式，使用[]'''
print(scores['张三'])  #输出为100

'''第二种方式，使用get()'''
print(scores,get('张三'))  #输出为100
print(scores,get('麻七',99))  #99是在查找‘麻七’所对的value不存在时，提供的一个默认值

#以上两种的区别为:第一种方法查找的键不存在是会给你报错的，但第二种方式不会报错，只会返回一个None
