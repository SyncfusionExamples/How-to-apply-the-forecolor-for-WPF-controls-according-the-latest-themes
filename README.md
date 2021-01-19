# How-to-apply-the-forecolor-for-WPF-controls-according-the-latest-themes
This repository contains the sample that how to apply the forecolor for WPF controls according the latest themes

To update the proper color for RibbonStatusBar text of Office2019 themes, the  Foreground property can be set based on the RibbonStatusBar Foreground property. Refer the below code for your reference

``` XAML

<syncfusion:RibbonWindow.StatusBar>
<syncfusion:RibbonStatusBar VerticalAlignment="Bottom">
<WrapPanel>
<TextBlock Text="Ready" Margin="10,0,0,0" Foreground="{Binding Path=Foreground, Mode=OneWay, RelativeSource={RelativeSource FindAncestor, AncestorType={x:Type syncfusion:RibbonStatusBar}}}" />
<TextBlock Text="Page No 1" Margin="20,0,0,0" />
</WrapPanel>
</syncfusion:RibbonStatusBar>
</syncfusion:RibbonWindow.StatusBar>
```

Output in Office2019White:

![RibbonStatusBar_Office2019White](Output_Office2019White.png)

Output in Office2019HighContrast:

![RibbonStatusBar_Office2019HighContrast](Output_Office2019HighContrast.png)
