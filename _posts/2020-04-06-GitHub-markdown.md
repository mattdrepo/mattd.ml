---
title: GitHub 的 markdown 语法
---

主题提供了完全兼容 GitHub 的 markdown 语法，你可以使用 GitHub 原生语法在本主题上写作。

本主题默认 markdown 渲染器是 [kramdown](https://kramdown.gettalong.org/)，在本主题的渲染效果如下

1. 目录
{:toc}

## 段落

在同个段落中，可以会出现不同的字体，包括但不限于：

1. 如果你要使用 `Italics` 斜体，可以在需要格式化的文字两边加上 `*`，例如

   ```markdown
   *The format of this sentence is italics*
   ```

2. 如果你要使用 `bold` 粗体，可以在需要格式化的文字两边加上 `**`，例如

   ```markdown
   **The format of the sentence is bold**
   ```

3. 如果你要给一段文字加上删除线，可以在需要格式化的文字两边加上 `--`，例如

   ```markdown
   --The format of this sentence is the deleted form--
   ```

4. <u>下划线</u>

当你需要换一个段落的时候，只需要按一下回车键即可。

## 链接

这个链接用 1 作为网址变量 [Google][1]
这个链接用 runoob 作为网址变量 [Runoob][runoob]
然后在文档的结尾为变量赋值（网址）

[1]: http://www.google.com/
[runoob]: http://www.runoob.com/

## 脚注

创建脚注格式类似这样 [^professordeng]。

[^professordeng]: 像我这样优秀的人。

## 引用

也许有时候你需要引用一下名人的话，这需要需要用到引用格式，通过在引用的话前面加 `>` 即可实现。例如

```markdown
> 没有人比我更懂政治。-- 特朗普
```

效果如下

> 没有人比我更懂政治。-- 特朗普

## 图片

也许文字不能更好地表达你的思想，可能需要图片来辅助，你可以通过 `![file-name](file-url)` 在你的文章中插入图片，效果如下

![大图]({{ site.cdn }}/big.jpg)

![小图]({{ site.cdn }}/small.jpg)

## 表格

当然有些数据比较复杂，你可能需要用到表格来列举，使用效果如下：

|       | mathematics | English | Chinese | Politics |
| ----- | ----------- | ------- | ------- | -------- |
| David | 80          | 80      | 50      | 100      |
| James | 70          | 80      | 90      | 100      |
| Me    | 100         | 90      | 100     | 100      |

超宽表格适配

|       | mathematics | English | Chinese | Politics | Japanese | python | basketball | javascript |
| ----- | ----------- | ------- | ------- | -------- | -------- | ------ | ---------- | ---------- |
| David | 80          | 80      | 50      | 100      | 98       | 100    | 99         | 1          |
| James | 70          | 80      | 90      | 100      | 12       | 90     | 88         | 2          |
| Me    | 100         | 90      | 100     | 100      | 120      | 50     | 77         | 3          |

## 代码

如果你是一个程序员，经常会需要核心代码来说明你的思路，所以为了方便程序员，我同样提供了高亮的代码格式，当公式行太长的时候，会自动水平滚动。例如 `js` 代码段格式如下，当然还包括很多其他编程语言的高亮，详细信息点击 [here](https://github.com/rouge-ruby/rouge/wiki/List-of-supported-languages-and-lexers)。

```js
 // Example can be run directly in your JavaScript console
 
 // Create a function that takes two arguments and returns the sum of those arguments
 var adder = new Function("a", "b", "return a + b");
 
 // Call the function
 adder(2, 6);
 // > 8
```

## 任务列表

无序号任务列表

- [x] This is a complete item
- [ ] This is an incomplete item

有序号任务列表

1. [x] This is a complete item
2. [ ] This is an incomplete item

## 表情

主题还支持 [emoji](https://emojipedia.org/) 表情。

- Nobody know more about technology than me
- 🙌没有人 👐比我 👌更懂 ☝科技

---