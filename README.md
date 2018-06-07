# OliveUI-Docs

用户对界面录入字段顺序的拖动自定义，分组自定义

show出自定义字段

## 主题变量

| 变量名 | 说明 |
| --- | --- |
| font-size-profile-context-menu | 侧写上下文菜单的字体大小 |
| font-size-menu-main-l1 | 主菜单字大小l1 |
| font-size-menu-main-l2 | 主菜单字大小l2 |
| font-size-menu-main-l3 | 主菜单字大小l3 |
| font-size-menu-main-l4 | 主菜单字大小l4 |
| font-size-toolbar-main-l1 | 主工具栏字大小l1 |
| font-size-toolbar-main-l2 | 主工具栏字大小l2 |
| font-size-toolbar-main-l3 | 主工具栏字大小l3 |
| bg-color-index-0 | 全局背景色/最底层背景色 |
| bg-color-toolbar-main | 主工具栏背景色 |
| bg-color-toolbar-sub | 子工具栏背景色 |
| tint-color-boolbar-main | 主工具栏前景色 |
| tint-color-boolbar-sub | 主工具栏前景色 |
| width-between-area-row | 区块之间的间距 |
| width-in-area-row | 区块内行间距 |
| icon-collapse-between-area | 区块间折叠的icon |
| icon-expand-between-area | 区块间展开的icon |


icon

大小

## 非主题变量

概念定义： 非主题变量是指该变量不应该跟随主题的变化而改变，但他仍然是变量可能由具体的项目自行调整。

## 区块

* 名称定义：

| 区块 | 标准名称 |
| --- | --- |
| 主工具栏区域 | oui-area-tool-bar |
| 表格工具栏区域 | oui-area-tool-bar-for-table |
| 搜索区 | oui-area-all-search |
| 主细表主表区域 | oui-area-main-common-edit |
| 主细表子表区域中的单条数据编辑界面 | oui-area-detail-common-edit |
| 列表和编辑在同一界面（AB类）的界面的明细编辑区域 | oui-area-ab1-detail-edit |

* 备忘笔记

area-main-common-edit:   主细表主表区域{
	三列或者四列，整站切换，要么整站三列要么整站四列（需要考虑，左边菜单展开的时候三列，收拢的时候四列），也有特殊情况，少数某几个页面可能通过后期用户配置决定到底是3列还是4列
	主表区域可能会有纵表（是独立页签还是和编辑界面融合，暂时不定）
}


area-detail-common-edit:   主细表子表区域中的单条数据编辑界面{
	
}

area-all-search:   搜索区{
	行数不确定
	
}

area-ab1-detail-edit:   界面的明细编辑区域{
	一个row只可能有一个分组
	可能有纵表
	可能有简单表格
}


区域与区域之间需要展开隐藏按钮


## 页面

* 命名规则：

    1. 页面的命名都是以字母开头，数字结尾，例如：a1。
    2. a表示列表类界面;b表示编辑类界面;ab表示同时具备列表和编辑界面，并且列表和编辑界面都是界面主要构成。

* 名称定义：

| 标准名称 | 说明 |
| --- | --- |
| oui-a1 | 结果集为单表的列表页面 |
| oui-a2 | 树加表格的列表页面 |
| oui-a3 | 树加主细表的列表页面 |
| oui-b1 | 结果集为单个表的编辑页面 |
| oui-b2 | 主细表的编辑页面 |
| oui-ab1 | 左边列表，右边编辑区的ab混合页面 |


* 备忘笔记
a1{
	
}
a2{
	
}
b1{
	
}
b2{
	
}

ab1{

}




## Complex控件
| 控件中文名 | 控件英文名 |
| --- | --- |
| 树控件 | ngx-first-tree |
| 工具栏控件 | ngx-tool-bar |
|  |  |


## 基本控件

基本控件基本上是继承Bootstrap，然后再进行重写一部分样式。