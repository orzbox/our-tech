# Matlab 绘图笔记

> 作者：[ScarboroughCoral](https://github.com/ScarboroughCoral)



总结整理一些常见数学函数和模型的绘制方法。



## 常用语法



### 匿名函数

```matlab
add=@(a,b) a+b
```





## 绘图



### 基础

#### 自然指数函数

```matlab
% function reference
myexp=@exp
x=0:0.2:5
plot(x,myexp(x))
```

![1547368133246](.\pics\1547368133246.png)

#### 自然指数函数积分

```matlab
syms x;
y=exp(x);
y=int(y);
ezplot(y);
```

![1547429452966](.\pics\1547429452966.png)

