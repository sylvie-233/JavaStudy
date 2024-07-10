# Groovy

## 基础介绍


### groovy
```
groovy:
    -v: 获取版本
```


### groovyConsole
GUI程序

```
```


## 核心内容

### 数据类型

兼容Java数据类型

def 定义动态类型

<br>

#### 字符串
单引号字符串：简单字符串

双引号字符串：可以变量插值

三引号字符串：原格式字符串



<br>

### 集合

#### List

基础使用
```groovy
// 定义列表（默认Java的ArrayList）
def list = [1, 2, 3]

// 列表添加元素
list << 4
```

<br>

#### Map

基础使用
```groovy
// 定义Map映射
def map = [key: value]

// map赋值
map.key = newValue
```




<br>

### 闭包

方法调用可以省略括号

Closure数据类型

<br>

基础使用
```groovy
// 闭包定义
def cl = {
    
}
```

