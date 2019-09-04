# HTML5-PDF.js
对HTML5 使用 PDF.js插件展示PDF文件的使用示例

# 使用方式：
无论哪种方式都是去访问/pdf/web/viewer.html这个文件，将PDF链接通过参数传递

1、a标签
'<a href="/pdf/web/viewer.html?file=file.pdf">Open</a>'

2、window.open跳转链接
window.open('/pdf/web/viewer.html?file=file.pdf','PDF','width:50%;height:50%');

3、iframe 内嵌页面打开
<iframe src="/pdf/web/viewer.html?file=file.pdf  name="PDF预览" marginwidth="15px" scrolling="no" sandbox="allow-scripts allow-same-origin" height="100%" width="100%"></iframe>

# 遇到问题：
Error:file origin does not match viewer's
打开web目录下的viewer.js文件
1794行注释掉：throw new Error('file origin does not match viewer\'s');
