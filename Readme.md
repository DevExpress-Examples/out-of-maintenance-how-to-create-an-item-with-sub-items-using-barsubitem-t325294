<!-- default badges list -->
![](https://img.shields.io/endpoint?url=https://codecentral.devexpress.com/api/v1/VersionRange/128640799/14.2.4%2B)
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/T325294)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
<!-- default badges end -->
<!-- default file list -->
*Files to look at*:

* [MainWindow.xaml](./CS/SubItemExample/MainWindow.xaml) (VB: [MainWindow.xaml](./VB/SubItemExample/MainWindow.xaml))
* [MainWindow.xaml.cs](./CS/SubItemExample/MainWindow.xaml.cs) (VB: [MainWindow.xaml.vb](./VB/SubItemExample/MainWindow.xaml.vb))
<!-- default file list end -->
# How to: Create an Item with Sub-Items Using BarSubItem


<p>This example demonstrates how to create an item with a sub-menu in its popup. To add bar items into <a href="https://documentation.devexpress.com/#WPF/clsDevExpressXpfBarsBarSubItemtopic">BarSubItem</a>, use the Items property:</p>


```xaml
<dxb:BarSubItem ...>
    <dxb:BarSubItem.Items>
        <dxb:BarButtonItem ...>
    </dxb:BarSubItem.Items>
</dxb:BarSubItem>
```


<p>Since Items is a content property, you can add other items directly into the BarSubItem tag:</p>


```xaml
<dxb:BarSubItem ...>
    <dxb:BarButtonItem .../>
</dxb:BarSubItem>
```


<p>If items are defined in another place, it's possible to reference a theme using the <a href="https://documentation.devexpress.com/#WPF/DevExpressXpfBarsBarSubItem_ItemLinkstopic">ItemLinks</a> property:</p>


```xaml
<dxb:BarManager>
    <dxb:BarManager.Items>
        <dxb:BarButtonItem Name="item1" .../>
    </dxb:BarManager.Items>
    ...
    <dxb:BarSubItem ...>
        <dxb:BarSubItem.ItemLinks>
            <dxb:BarButtonItemLink BarItemName="item1"/>
        </dxb:BarSubItem.ItemLinks>
    </dxb:BarSubItem>
</dxb:BarManager>
```



<br/>


