# TicketDivideLine
仿各种卡票分割线、电影票分割线。支持自定义分割线长度、分割线间隔长度、分割线颜色、方向等属性。

[![](https://jitpack.io/v/kjt666/TicketDivideLine.svg)](https://jitpack.io/#kjt666/TicketDivideLine)

使用
-----
要在您的构建中获得Git项目：<br>

步骤1.将JitPack存储库添加到构建文件中<br>

将其添加到存储库末尾的根build.gradle中：<br>

```Java
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```
步骤2.添加依赖项<br>

```Java
dependencies {
	        implementation 'com.github.kjt666:TicketDivideLine:v1.1'
	}
```

演示
-----
![](https://github.com/kjt666/Images/blob/master/TicketDivideLine.png)
```Java
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="150dp"
        android:background="#ffffff">

        <wowo.kjt.library.TicketDivideLine
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginTop="40dp" />

    </LinearLayout>

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="150dp"
        android:layout_marginTop="10dp"
        android:background="#ffffff">

        <wowo.kjt.library.TicketDivideLine
            android:layout_width="wrap_content"
            android:layout_height="match_parent"
            android:layout_marginLeft="70dp"
            app:line_orientation="line_vertical" />

    </LinearLayout>
 ```
 属性说明
 -----
 * divid_line_color：<br>
 分割线颜色
 * divide_line_length：<br>
 分割线实线长度
 * divide_line_interval：<br>
 分割线虚线长度（间隔长度）
 * port_shape_diameter：<br>
 两端半圆缺口直径
 * port_shape_color：<br>
 两端半圆缺口颜色
 * line_orientation：<br> 
    line_vertical<br>
    line_horizontal<br>
    分割线方向，有水平和垂直方向，和LinearLayout的orientation一样。
