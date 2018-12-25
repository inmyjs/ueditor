# ueditor
优化百度ueditor编辑器，增加秀米插件、手机端预览等功能，与egg-ueditor完美结合

### 主要优化项
1. 关闭了多余的功能项，主要针对手机端内容编辑；
2. 原来很Low的图标替换了（这是抄别人的）；
3. 增加秀米插件，内容编辑真是方便啊，如果有秀米vip的就更好使了；
4. 增加手机端预览功能，方便检查内容；
5. 关闭了本地保存成功的提示，仅关闭了提示。
6. 与egg-ueditor完美结合。

效果图：

![](https://raw.githubusercontent.com/wiki/inmyjs/ueditor/images/1.png)
![](https://raw.githubusercontent.com/wiki/inmyjs/ueditor/images/2.png)
![](https://raw.githubusercontent.com/wiki/inmyjs/ueditor/images/3.png)

### 使用方法
1. 下载源码，放至静态资源目录
2. 在页面引用
``` html
<!DOCTYPE html>
<html>
<head>
<script src="/public/ueditor/ueditor.config.js"></script>
<script src="/public/ueditor/ueditor.all.js"></script>
<script src="/public/ueditor/xiumi-ue-dialog-v5.js"></script>
<link rel="stylesheet" href="/public/ueditor/xiumi-ue-v5.css">
  </head>
  <body>
    <h1>编辑器示例</h1>
    <div id="content"></div>
    <script type="application/javascript">
      let ueditor_config = {
        serverUrl: "/ueditor?_csrf={{ ctx.csrf | safe }}",
        initialFrameWidth: 700,
        initialFrameHeight: 320,
        autoHeightEnabled: false
      };
      var ue = UE.getEditor('content',ueditor_config);
    </script>
  </body>
</html>
```
3. 详细使用见ueditor官方文档

### 非常感谢您的支持
撸码不易，如果对你有所帮助，欢迎您的赞赏！微信赞赏码：

![](https://raw.githubusercontent.com/wiki/inmyjs/asweb/images/20180831154543.jpg)
