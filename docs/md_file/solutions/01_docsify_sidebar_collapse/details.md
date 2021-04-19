# docsify 侧边栏目录扩展

## 1、设置侧边栏目录最大层级
与配置loadSidebar一起使用，根据打开的md文中的#的个数，生成目录结构。
1：不生成目录直接，只显示md文件的标题
2：根据只有一个#的内容，生成目录结构
3：生成一个#的目录，再生成两个#的目录
以此类推
```
subMaxLevel: 2
```
![设置侧边栏目录最大层级](./images/image001.png)

运行效果
![设置侧边栏目录最大层级](./images/image002.png)

设置为3的时候的效果
```
subMaxLevel: 3
```
![设置侧边栏目录最大层级](./images/image003.png)

运行效果
![设置侧边栏目录最大层级](./images/image004.png)

## 2、开启侧边栏的折叠功能
使用一个开源代码，在index.html添加js插件
```javascript
<script src="//cdn.jsdelivr.net/npm/docsify-sidebar-collapse/dist/docsify-sidebar-collapse.min.js"></script>
```
![开启侧边栏的折叠功能](./images/image005.png)

运行效果
![开启侧边栏的折叠功能](./images/image006.png)

![开启侧边栏的折叠功能](./images/image007.png)

可以使用sidebarDisplayLevel设置默认折叠的层级
```javascript
sidebarDisplayLevel: 1
```
![开启侧边栏的折叠功能](./images/image008.png)

## 3、给侧边栏添加样式
导入一级菜单的样式
```javascript
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify-sidebar-collapse/dist/sidebar.min.css" />
```
![给侧边栏添加样式](./images/image009.png)

运行效果
![给侧边栏添加样式](./images/image010.png)

![给侧边栏添加样式](./images/image011.png)

导入二级菜单的样式
```javascript
<link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify-sidebar-collapse/dist/sidebar-folder.min.css" />
```
![给侧边栏添加样式](./images/image012.png)

运行效果
![给侧边栏添加样式](./images/image013.png)

![给侧边栏添加样式](./images/image014.png)

## 4、将JS和CSS下载到本地，从本地进行加载
```
下载地址：
https://github.com/iPeng6/docsify-sidebar-collapse
```
![下载源代码](./images/image015.png)

下载到本地
![下载源代码](./images/image016.png)

将下载的源代码，拷贝到docs文件夹下面
![下载源代码](./images/image017.png)

修改引入源代码的代码
![下载源代码](./images/image018.png)