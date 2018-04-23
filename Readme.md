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


