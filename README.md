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

```<Viewerjs />```

单图片+简化工具条

```<Viewerjs Src="@_srcPhoto" Width="600px" Height="300px" toolbarlite="true" />```

多图片+简化工具条

```<Viewerjs Images='new List<string>() { "photo-2.jpg","photo-1.jpg","photo-3.jpg"}' toolbarlite="true" />```

多图片

```<Viewerjs Images='new List<string>() { "photo-2.jpg","photo-1.jpg","photo-3.jpg"}' />```

