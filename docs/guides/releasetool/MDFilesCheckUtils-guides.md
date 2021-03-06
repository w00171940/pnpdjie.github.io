---
title: 低检工具使用说明
---

{% capture article %}

## 使用步骤

1. 将jekyll项目下载到本地。（具体下载方式请参考jekyll相关文档）  
2. 点击右上方的“select file”按钮，在弹出窗口中选择jekyll项目的根路径文件夹，并确定  
![](/images/docs/guides/releasetool/2.1.1_1.png "低检工具_使用")  
3. 选择左侧的“低检”选项框，点击“start check”按钮，等待项目检测完成。正下方的进度条会同步显示总文件数和已检测的文件数量。  
4. 检测完成后，界面中会显示各个检测项目的结果总数、处理建议以及日志保存路径。如下图所示：  
![](/images/docs/guides/releasetool/2.1.1_2.png "低检工具_使用")  
5. 想要查看详细结果，可以点击左上方的“browse log”按钮，会自动打开检查结果日志。  

## 检测项目及处理建议

### 1. 失效链接

说明此链接无法通过网络正常访问，原因可能为链接被删除、链接地址错误或断网等原因导致。  
**处理建议**：请检查本地网络是否通畅，链接是否输入正确，若链接被删除，请删除或改用其他网页链接替代。

### 2. 错误include标签引用路径

页面中所有的include标签中错误的路径，如：{% include templates/home.md %}中，如果项目的/_include/templates文件夹中并没有home.md文件，则会在结果中显示出来。  
**处理建议**：请检查项目相对路径是否输入正确，或者原文件是否被删除。

### 3. 错误内部引用路径

页面中用“[链接文字](文件路径)”的md格式引入本地文件时，路径错误。原因可能因为本地文件路径错误，或者被引用的文件被删除。  
**处理建议**：请检查项目相对路径是否输入正确，或者原文件是否被删除。

### 4. 字符编码不正确

说明此文件的编码格式不符合项目要求。  
**处理建议**：请用编辑工具将文件的字符编码转换为合适的编码格式，建议为UTF-8格式，否则可能出现乱码。

### 5. title格式不正确

说明此文件的title部分格式错误。  
**处理建议**：请修改为正确的格式。格式要求如下：
1. 起始和结束的短横线都应为3个，不能多不能少，也不能有空格。  
2. 中间内容部分应为键值对格式，key和value中间用英文格式冒号后紧跟一个英文空格隔开。  
正确实例如下：  

		---
		title: this is title
		---

## 注意事项

1. 检测热点链接原理是向所有的链接发送网络请求，并根据返回信息判断链接是否失效，因此耗费时间较长。  
2. 检测需要打通外网环境，否则所有的热点链接会全部标识为失效链接。  
3. 检测Include标签内的引用路径原理是根据根目录判断引用文件是否存在，因此选择项目根路径时一定要选择正确，否则所有的include标签引用路径会全部标识为错误路径。


{% endcapture %}

{% include templates/home.md %}
