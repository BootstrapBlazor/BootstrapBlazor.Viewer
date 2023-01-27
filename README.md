# Blazor Viewer 图片浏览器 组件

封装Viewer.js库

示例:

https://blazor.app1.es/viewer

使用方法:

1.nuget包

```BootstrapBlazor.Viewer```

2._Imports.razor 文件 或者页面添加 添加组件库引用

```@using BootstrapBlazor.Components```


3.razor页面

Demo

`<Viewerjs />`

多图片

`<Viewerjs Images='new List<string>() { "photo-2.jpg","photo-1.jpg","photo-3.jpg"}' />`

单图片

`<Viewerjs Src="@_srcPhoto" Width="600px" Height="300px" />`

单图片+简化工具条

`<Viewerjs Src="@_srcPhoto" Width="600px" Height="300px" toolbarlite="true" />`

多图片+简化工具条

`<Viewerjs Images='new List<string>() { "photo-2.jpg","photo-1.jpg","photo-3.jpg"}' toolbarlite="true" />`

单图片流

`<Viewer SrcStream="imagesStreamList[1]" />`

多图片流

`<Viewer ImagesStream="imagesStreamList" />`

本地单图片,组件流读取

`<Viewer Src='@(@"F:\images\objects.jpg")' LocalFileToStream />`

4.参数说明 


|  类型   |  参数   | 说明  | 默认值  | 备注  |
|  ----  | ----  | ----  |  ----  |  ----  | 
| bool | UseBuiltinImageDiv  | 使用内置图片DIV | true |  |
| List&lt;string&gt; | Images  | 图片列表DIV |  |  |
| string | Src | 单图片 |  |  |
| List&lt;string&gt; | Alts | 图片名称列表 |  |  |
| bool |toolbarlite | 简化版工具条 | false |  |
| string | Height | 高 | 400px |  |
| string | Width | 宽 | 400px |  |
| string | ID | 组件ID |  |  |
| List&lt;Stream&gt; | ImagesStream | 图片流列表 |  |  |
| Stream | SrcStream | 单图片流 |  |  |
| bool | LocalFileToStream | 使用流读取本地图片 | false |  |

---
#### 更新历史

v7.0.2
- 支持流转图片(ImageFromStream), 用于本地项目例如 MAUI Blazor,Blazor hybrid,因为chorome不支持file:///xx 方式显示本地图片
- 添加 ImagesStream : 图片流列表
- SrcStream : 单图片流
- LocalFileToStream : 使用流读取本地图片

----

#### Blazor 组件

[条码扫描 ZXingBlazor](https://www.nuget.org/packages/ZXingBlazor#readme-body-tab)
[![nuget](https://img.shields.io/nuget/v/ZXingBlazor.svg?style=flat-square)](https://www.nuget.org/packages/ZXingBlazor) 
[![stats](https://img.shields.io/nuget/dt/ZXingBlazor.svg?style=flat-square)](https://www.nuget.org/stats/packages/ZXingBlazor?groupby=Version)

[图片浏览器 Viewer](https://www.nuget.org/packages/BootstrapBlazor.Viewer#readme-body-tab)
  
[条码扫描 BarcodeScanner](Densen.Component.Blazor/BarcodeScanner.md)
   
[手写签名 Handwritten](Densen.Component.Blazor/Handwritten.md)

[手写签名 SignaturePad](https://www.nuget.org/packages/BootstrapBlazor.SignaturePad#readme-body-tab)

[定位/持续定位 Geolocation](https://www.nuget.org/packages/BootstrapBlazor.Geolocation#readme-body-tab)

[屏幕键盘 OnScreenKeyboard](https://www.nuget.org/packages/BootstrapBlazor.OnScreenKeyboard#readme-body-tab)

[百度地图 BaiduMap](https://www.nuget.org/packages/BootstrapBlazor.BaiduMap#readme-body-tab)

[谷歌地图 GoogleMap](https://www.nuget.org/packages/BootstrapBlazor.Maps#readme-body-tab)

[蓝牙和打印 Bluetooth](https://www.nuget.org/packages/BootstrapBlazor.Bluetooth#readme-body-tab)

[PDF阅读器 PdfReader](https://www.nuget.org/packages/BootstrapBlazor.PdfReader#readme-body-tab)

[文件系统访问 FileSystem](https://www.nuget.org/packages/BootstrapBlazor.FileSystem#readme-body-tab)

[光学字符识别 OCR](https://www.nuget.org/packages/BootstrapBlazor.OCR#readme-body-tab)

[电池信息/网络信息 WebAPI](https://www.nuget.org/packages/BootstrapBlazor.WebAPI#readme-body-tab)

[视频播放器 VideoPlayer](https://www.nuget.org/packages/BootstrapBlazor.VideoPlayer#readme-body-tab)

#### AlexChow

[今日头条](https://www.toutiao.com/c/user/token/MS4wLjABAAAAGMBzlmgJx0rytwH08AEEY8F0wIVXB2soJXXdUP3ohAE/?) | [博客园](https://www.cnblogs.com/densen2014) | [知乎](https://www.zhihu.com/people/alex-chow-54) | [Gitee](https://gitee.com/densen2014) | [GitHub](https://github.com/densen2014)