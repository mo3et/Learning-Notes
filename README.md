# Learning-Note

## About Git
git config --global user.name

git config --global user.email

git pull --rebase origin master

pull 这条指令的意思是把远程库中的更新合并到本地库中，–rebase的作用是取消掉本地库中刚刚的commit，并把他们接到更新后的版本库之中

git pull –rebase origin master意为先取消commit记录，并且把它们临时 保存为补丁(patch)(这些补丁放到”.git/rebase”目录中)，之后同步远程库到本地，最后合并补丁到本地库之中。

# Markdown 教程

    ##  other
        1. 实现缩进
        两种方案
    
        手动输入空格 （&nbsp；）。注意！此时的分号为英文分号，但是不推荐使用此方法，太麻烦！
    
        使用全角空格(切换快捷键shift+空格)。即：在全角输入状态下直接使用空格键就ok了
    
        2. 实现换行
        两种方案
    
        两个空格加回车即可  
    
        使用< br >
    
        3. 字体大小、颜色、类型、加粗、倾斜
        < font size=5> Hello
    
        < font color=red>color
    
        < font face=“微软雅黑”>微软雅黑
    
        ** 内容 ** 　(*与内容之间没有空格)
    
        *内容 * 　　 (*与内容之间没有空格)
    
        4. 代码块
        (```)
    
        int a = 0 ;
    
        System.out.println(“Hello”) ;
    
        (```)
    
        注意！为了防止转译，前后三个反引号处加了小括号，实际是没有的。
    
        5. 超链接
        [超链接名] (超链接地址 “超链接title”)
    
        [百度] (http://baidu.com) （注意！[]与()之间没有空格）
    
        6. 分割线
        三个或者三个以上的 - 或者 * 都可以。
        7. 标题
        通过在文字前面添加#即可


        # 这是一级标题
    
        ## 这是二级标题
    
        ### 这是三级标题


## 0. 有关字体  
*斜体文本*  
_斜体文本_  
**粗体文本**  
__粗体文本__  
***粗斜体文本***  
___粗斜体文本___  

**不换行空格**    
&nbsp;不换行空格  
**半角空格**  
 &ensp;半角空格  
 **全角空格**  
  <br>--换行--
&emsp;全角空格  

## 1. 换行规范  

换行是两个空格加enter  
例 this

或者使用一个空行来表示重新开始一个段落（两个enter）

## 2.分割线  

    ***
    * * *
    *****
    - - -
    ----------

## 3.删除线  
如果段落上的文字要添加删除线，只需要在文字的两端加上两个波浪线 ~~ 即可，实例如下：

GOOGLE.COM  
~~BAIDU.COM~~

## 4.下划线
下划线可以通过 HTML 的 <u> 标签来实现：

<u>带下划线文本 </u></u>

## 5.脚注
脚注是对文本的补充说明。  
Markdown 脚注的格式如下:
[^要注明的文本]  
例：  
This is a [^Footnote]  

[^Footnote]: 脚注 提供的注释 (适用于typora,但vscode好像不适用)

## 6. MD列表  
支持无序列表和有序列表
### 无序列表  
无序列表使用星号(*)、加号(+)或是减号(-)作为列表标记：  
例：
* 第一列
* 第二列  

+ 第三列
+ 第四列

- 第五列
- 第六列  
### 有序列表
有序列表使用数字并加上 . 号来表示，如：
1. 第一项
2. 第二项
3. 第三项

### 列表嵌套  
列表嵌套只需在子列表中的选项添加四个空格(或 tab)即可：

1. 第一项：
    - 第一项嵌套的第一个元素
    - 第一项嵌套的第二个元素
2. 第二项：
    - 第二项嵌套的第一个元素
    - 第二项嵌套的第二个元素
3. 第三项：
    - test

## 7. Markdown 区块  
Markdown 区块引用是在段落开头使用 > 符号 ，然后后面紧跟一个空格符号：  
例：
 >such as  
 >is   
 >it

 另外区块是可以嵌套的，一个 > 符号是最外层，两个 > 符号是第一层嵌套，以此类推：
> 最外层
> > 第一层嵌套
> > > 第二层嵌套

### 区块中使用列表
区块中使用列表实例如下：
> 区块中使用列表
> 1. 第一项
> 2. 第二项
> + 第一项
> + 第二项
> + 第三项

### 列表中使用区块
如果要在列表项目内放进区块，那么就需要在 > 前添加四个空格的缩进。
区块中使用列表实例如下：
* 第一项
    > insert 区块  
    > 区块2
* 第二项

## 7. Markdown 代码
如果是段落上的一个函数或片段的代码可以用反引号把它包起来（`），例如：`

`printf()` 函数

### 代码区块
代码区块使用 4 个空格或者一个制表符（Tab 键）。  
实例如下:
    
    printf("this is code area ")

你也可以用 ``` 包裹一段代码，并指定一种语言（也可以不指定）：
```javascript
$(document).ready(function () {
    alert('Code');
});
```
```C
#include<stdio.h>
int main(){
    printf("Hello Markdown");
    return 0;
}
```

## 8.Markdown 链接
链接使用方法如下：
[链接名称](链接地址)  
或者  
<链接地址>
<https://github.com/Mo3et>  
例如：
This is my Github. [My Github](https://github.com/Mo3et)

### 高级链接  
链接也可以用变量来代替，文档末尾附带变量地址：  
这个链接用 1 作为网址变量 [Github][1]  
这个链接用 github 作为网址变量 [MyGithub][github]  
然后在文档的结尾为变量赋值（网址）  
[1]: http://www.github.com/  
[github]: http://www.github.com/Mo3et

## 9.Markdown 图片
Markdown 图片语法格式如下：

![alt 属性文本](图片地址)

![alt 属性文本](图片地址 "可选标题")
开头一个感叹号 !  
接着一个方括号，里面放上图片的替代文字  
接着一个普通括号，里面放上图片的网址，最后还可以用引号包住并加上选择性的 'title' 属性的文字。

![My github image](https://avatars1.githubusercontent.com/u/34803812?s=460&v=4 "头像")

当然，你也可以像网址那样对图片网址使用变量  
这个链接用 1 作为网址变量 [Github image][1].  
然后在文档的结尾为变量赋值（网址）
[1]: https://avatars1.githubusercontent.com/u/34803812?s=460&v=4


Markdown 还没有办法指定图片的高度与宽度，  
如果你需要的话，你可以使用普通的 <img> 标签。

<img src="https://avatars1.githubusercontent.com/u/34803812?s=460&v=4" width="50%">

## 9. Markdown 表格  
Markdown 制作表格使用 | 来分隔不同的单元格，使用 - 来分隔表头和其他行。  
语法格式如下：
|  表头   | 表头  |
|  ----  | ----  |
| 单元格  | 单元格 |
| 单元格  | 单元格 |

### 对齐方式
我们可以设置表格的对齐方式：  
-: 设置内容和标题栏居右对齐。  
:- 设置内容和标题栏居左对齐。  
:-: 设置内容和标题栏居中对齐。  
实例如下：

| 左对齐 | 右对齐 | 居中对齐 |
| :-----| ----: | :----: |
| 单元格 | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 |

## Markdown 高级技巧
### 支持的 HTML 元素
不在 Markdown 涵盖范围之内的标签，都可以直接在文档里面用 HTML 撰写。

目前支持的 HTML 元素有：<kbd> <b> <i> <em> <sup> <sub> <br>等 ，如：

使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑

### 转义
Markdown 使用了很多特殊符号来表示特定的意义，如果需要显示特定的符号则需要使用转义字符，Markdown 使用反斜杠转义特殊字符：  

        **文本加粗**   

        \*\* 正常显示星号 \*\*
#### Markdown 支持以下这些符号前面加上反斜杠来帮助插入普通的符号：

        \   反斜线
        `   反引号
        *   星号
        _   下划线
        {}  花括号
        []  方括号
        ()  小括号
        #   井字号
        +   加号
        -   减号
        .   英文句点
        !   感叹号

### 公式
当你需要在编辑器中插入数学公式时，可以使用两个美元符 $$ 包裹 TeX 或 LaTeX 格式的数学公式来实现。提交后，问答和文章页会根据需要加载 Mathjax 对数学公式进行渲染。如：

        $$
        \mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
        \mathbf{i} & \mathbf{j} & \mathbf{k} \\
        \frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
        \frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
        \end{vmatrix}
        ${$tep1}{\style{visibility:hidden}{(x+1)(x+1)}}
        $$



        