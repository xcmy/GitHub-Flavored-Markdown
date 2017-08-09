## GitHub上项目README.md文件编写常用语法介绍

README使用的是[GitHub Flavored Markdown](https://github.github.com/gfm/)，是markdowm语法的扩展。简称GFM。

[Markdown中文文档](http://wowubuntu.com/markdown/)

[Markdown英文文档](https://daringfireball.net/projects/markdown/basics)


以下介绍了GFM常用语法写法以及效果展示。

## 目录

- [横线](#横线)
- [标题](#标题)
- [文本](#文本)
- [图片](#图片)
- [链接](#链接)
- [列表](#列表)
- [块引用](#块引用)
- [代码高亮](#代码高亮)



### 横线


横线 | 写法
---|---
1 | ***
2 | ---
3 | ___

效果依次为(没多大区别)

***
---
___


### 标题

标题 | 写法
---|---
一级标题 | # XXX
二级标题 | ## XXX
三级标题 | ### XXX
四级标题 | #### XXX
五级标题 | ##### XXX
六级标题 | ###### XXX

效果如下
# XXX
## XXX
### XXX
#### XXX
##### XXX
###### XXX

### 文本

文本 | 写法|效果
---|---|---
普通文本 | 文本 |hello world
单行文本 | （tab或4空格）+文本 | 见下面效果
文本块1 | 每行（tab或4空格）+文本 |见下面效果
文本块2 | 用 ``` 把文本包起来 | 见下面效果
文字高亮|用`把文字包起来 | 见下面效果
换行|文本间加两个空格或者空行 | 见下面效果
斜体1 | `*hello*` | *hello*
斜体2 | `_hello_` | _hello_
粗体1 | `**hello**` | **hello**
粗体2 | `__hello__`| __hello__
删除线| `~~hello~~`| ~~hello~~
斜粗体1 | `***hello***`| ***hello***
斜粗体2 | `___hello___`| ___hello___
斜粗体删除线1 |`***~~hello~~***` |***~~hello~~***
斜粗体删除线2 |`~~***hello***~~`|~~***hello***~~

效果如下

- 普通文本

 hello world

- 单行文本


    hello world

- 文本块1


    hello !
    welcome to beijing.

- 文本块2


```
hello !
welcome to beijing.

```
    
- 文字高亮

`3333`
`hello`
`你好`

- 换行

hello  
world


### 图片


图片 | 写法
---|---
1 | `![image](URL title)`

效果

![image](https://avatars1.githubusercontent.com/u/9919?v=4&s=200)

### 链接

链接 | 写法 |效果 |备注
---|---|---|---
外部链接 | `[百度一下](https://www.baidu.com/)`|[百度一下](https://www.baidu.com/) | --
项目内文件链接 | `[README](./README.md)`|[README](./README.md) | --
文件内锚点链接（中文） | `[返回顶部](#目录)` |[返回顶部](#目录) | --
文件内锚点链接（英文） | `[返回底部](#bottom-out)` |[返回底部](#bottom-out) | 标题大写用小写代替，空格用-代替
	

### 列表

##### 无序列表
###### 写法

    - 小明
    - 小红
    - 小刚

###### 效果

- 小明
- 小红
- 小刚

#####  多行无序列表

###### 写法

    - 第一章
      - 第一节
        - 第一小节
      - 第二节
    - 第二章


###### 效果

 - 第一章
      - 第一节
        - 第一小节
      - 第二节
 - 第二章
 
##### 有序列表

###### 写法

    1. 第一步
    1. 第二步
    1. 第三步
    
或

    1. 第一步
    2. 第二步
    2. 第三步
    
###### 效果
1. 第一步
1. 第二步
1. 第三步


##### 多级有序列表
###### 写法

    1. 第一步
       1. 第一小步
            1. 第一小小步
            2. 第二小小步
       2. 第二小步
    1. 第二步
    
###### 效果（二级罗马数字，三级英文字母）
1. 第一步
   1. 第一小步
        1. 第一小小步
        2. 第二小小步
   2. 第二小步
1. 第二步
    

#####  复选框

###### 写法

    - [x] 任务一
    - [x] 任务二
    - [x] 任务三
    - [ ] 任务四
    - [ ] 任务五
    - [ ] 任务六
    
###### 效果

- [x] 任务一
- [x] 任务二
- [x] 任务三
- [ ] 任务四
- [ ] 任务五
- [ ] 任务六

### 块引用

###### 写法

    > 文本
    
###### 效果

>I have a dream that my four little children will one day live in a nation where they will not be judged by the color of their skin but by the content of their character.  
I have a dream today!  
 --马丁·路德·金


### 代码高亮

###### 写法
json

    ```json
    {
    "_id":"1",
    "name":"小明"
    }
    ```  
swift

    ```Swift
    var name:String = "小明"
    ```
###### 效果 

```json
    {
    "_id":"1",
    "name":"小明"
}
```
```Swift
    var name:String = "小明"
```



### Bottom Out