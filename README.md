# 三凡物联网服务器协议说明文档
服务器通信使用基于**http**的**rest**协议，并不完全准守restful规范标准。  
根据实际情况设计服务器内部和外部的协议规则。   
## 全局默认说明 ##
### 数据格式 ###
- **所有数据为json格式**  
string化的json，buffer化的json，或者json本身  
如果请求失败则返回**{ret:原因编码}**
### 默认参数 ###
- **参数中带project字段以区分项目**  
比如**?project=ligong_water**


## 内部协议 localhost ##
### MongoDB协议 端口41111 ###
- **/add 增加数据**  
body：json  

- **/history 取得历史数据**  
参数：skip跳过的数据数量，limit取得多少数据  
body：无   
返回：json  

- **/total 数据数量**  
参数：无  
body：无  
返回：json  

### 大数据模块 端口30911 ###
- **/search** 
参数：无  
body：无  
操作：取得数据总量  
返回：json  

### WebSocket模块 ###
- **/项目名称** 
- **rest监听**

# protocol
protocol for restful
## Welcome to MarkdownPad 2 ##

**MarkdownPad** is a full-featured Markdown editor for Windows.

### Built exclusively for Markdown ###

Enjoy first-class Markdown support with easy access to  Markdown syntax and convenient keyboard shortcuts.

Give them a try:

- **Bold** (`Ctrl+B`) and *Italic* (`Ctrl+I`)
- Quotes (`Ctrl+Q`)
- Code blocks (`Ctrl+K`)
- Headings 1, 2, 3 (`Ctrl+1`, `Ctrl+2`, `Ctrl+3`)
- Lists (`Ctrl+U` and `Ctrl+Shift+O`)

### See your changes instantly with LivePreview ###

Don't guess if your [hyperlink syntax](http://markdownpad.com) is correct; LivePreview will show you exactly what your document looks like every time you press a key.

### Make it your own ###

Fonts, color schemes, layouts and stylesheets are all 100% customizable so you can turn MarkdownPad into your perfect editor.

### A robust editor for advanced Markdown users ###

MarkdownPad supports multiple Markdown processing engines, including standard Markdown, Markdown Extra (with Table support) and GitHub Flavored Markdown.

With a tabbed document interface, PDF export, a built-in image uploader, session management, spell check, auto-save, syntax highlighting and a built-in CSS management interface, there's no limit to what you can do with MarkdownPad.


