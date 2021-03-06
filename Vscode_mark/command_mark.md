#! https://zhuanlan.zhihu.com/p/503790154
[TOC]
#### 字体
```markdown
**加粗**   *斜体*  ~~删除线~~   ==高亮==
```
效果：**重点加粗**$\quad$*斜体*$\quad$~~删除线~~$\quad$==高亮==
选中文字按`ctrl+B`粗体,`ctrl+I`斜体
#### 列表
```markdown
* 无序列表
    * 嵌套列表1
    * 嵌套列表2
      * 嵌套
1. 有序列表
   1. 有序嵌套
   2. 有序嵌套
2. 有序列表2
```
* 无序列表
    * 嵌套列表1
    * 嵌套列表2
      * 嵌套

1. 有序列表
   1. 有序嵌套
   2. 有序嵌套
2. 有序列表2

快捷键 `ctrl+[` 退格，`ctrl+]`嵌套缩进


任务列表
```markdown
- [x] 已经完成的事
- [ ] 未完成的事
```
- [x] 已经完成的事
- [ ] 未完成的事
#### 引用和代码
引用：
```markdown
> 引用别人的话
就这样
直到回车结束
```
> 引用别人的话
就这样
直到回车结束

防止转译：
```markdown
`行内代码`
\`不转译\`
```
效果：`行内代码` $\quad$ \`不转译\`

代码块语法：
>\```c++
static int a;
\```

其中代码语言类型如python,java,c++等可以让代码块中的代码关键字高亮，效果：
```c++
static int a;
```
代码块也可显示代码行数，在语言类型后面加{.line-numbers}即可：
>\```c++ {.line-numbers}
int function(int a,int b){
    return a+b;
}
\```

效果：
```c++ {.line-numbers}
int function(int a,int b){
    return a+b;
}
```
#### 超链接和图片
使用如下语法插入图片或超链接
使用网址：
```markdown
[b站网址](https://www.bilibili.com/) 
![赛罗](images/Zero.png)
```
[b站网址](https://www.bilibili.com/)
<div align=center>
    <img width='640' src="images/Zero.png">
</div>

使用本地地址(注意放在本`.md`文件夹下):
```markdown
[brief_introduction.md](math_mark.md)
![柯南](images/Conan.jpg)
```
[brief_introduction.md](math_mark.md)
![柯南](images/Conan.jpg)

为方便起见，安装了`Paste Image`插件，再按`ctrl+,`打开设置，输入`Paste Image Path`把对应的代码改成`${currentFileDir}/images`即可，之后便可使用快捷键`Ctrl+Alt+V`粘贴图片。
为了调整图片大小和对齐，使多张图片在同一行，可以采用HTML语言：
```html
<div align=center>
    <img width='220' height='144' src="images/柯南.jpg">
</div>
/****/
<div align=center>
    <img src="images/柯南.jpg" width='30%'>
    <img src="images/柯南.jpg" width='30%'>
    <img src="images/柯南.jpg" width='30%'>
</div>
```
<div align=center>
    <img src="images/柯南.jpg" width='220'>
</div>
<div align=center>
    <img src="images/柯南.jpg" width='30%'>
    <img src="images/柯南.jpg" width='30%'>
    <img src="images/柯南.jpg" width='30%'>
</div>

#### 表格
```markdown
| 表头 | 表头 |
| ---- | ---- |
| 内容 | 内容 |
| 内容 | 内容 |
```
| 表头 | 表头 |
| ---- | ---- |
| 内容 | 内容 |
| 内容 | 内容 |
合并单元格等操作需要使用HTML：
```html
<table style="text-align:center">
    <tbody>
        <tr>
            <th rowspan='2'> </th>
            <th colspan='3'>欧拉角</th>
            <th colspan='3'>xyz移动</th>
        </tr>
        <tr>
            <th>alpha</th>
            <th>beta</th>
            <th>gamma</th>
            <th>x</th>
            <th>y</th>
            <th>z</th>
        </tr>
        <tr>
            <th rowspan='2'>第一组</th>
            <td>0</td>
            <td>10°</td>
            <td>20°</td>
            <td>1</td>
            <td>2</td>
            <td>3</td>
        </tr>
        <tr>
            <td>0</td>
            <td>110°</td>
            <td>120°</td>
            <td>11</td>
            <td>12</td>
            <td>13</td>
        </tr>
        <tr>
            <th rowspan='2'>第二组</th>
            <td>0</td>
            <td>30°</td>
            <td>40°</td>
            <td>5</td>
            <td>6</td>
            <td>7</td>
        </tr>
        <tr>
            <td>0</td>
            <td>130°</td>
            <td>140°</td>
            <td>15</td>
            <td>16</td>
            <td>17</td>
        </tr>
    </tbody>
</table>
```
<table style="text-align:center">
    <tbody>
        <tr>
            <th rowspan='2'> </th>
            <th colspan='3'>欧拉角</th>
            <th colspan='3'>xyz移动</th>
        </tr>
        <tr>
            <th>alpha</th>
            <th>beta</th>
            <th>gamma</th>
            <th>x</th>
            <th>y</th>
            <th>z</th>
        </tr>
        <tr>
            <th rowspan='2'>第一组</th>
            <td>0</td>
            <td>10°</td>
            <td>20°</td>
            <td>1</td>
            <td>2</td>
            <td>3</td>
        </tr>
        <tr>
            <td>0</td>
            <td>110°</td>
            <td>120°</td>
            <td>11</td>
            <td>12</td>
            <td>13</td>
        </tr>
        <tr>
            <th rowspan='2'>第二组</th>
            <td>0</td>
            <td>30°</td>
            <td>40°</td>
            <td>5</td>
            <td>6</td>
            <td>7</td>
        </tr>
        <tr>
            <td>0</td>
            <td>130°</td>
            <td>140°</td>
            <td>15</td>
            <td>16</td>
            <td>17</td>
        </tr>
    </tbody>
</table>



#### 注释
使用快捷键`ctrl+\`将当前行注释，`ctrl+/`取消注释
```markdown
<!--注释内容-->
<!--多行内容
注释-->
```
<!--注释内容-->
<!--多行内容
注释-->