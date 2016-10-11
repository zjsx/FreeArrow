# FreeArrow
Android可以自定义颜色和形状的箭头，可以用作导航键头等，避免使用各种颜色的箭头PNG.
![](https://github.com/zjsx/FreeArrow/blob/master/screenshot/Screenshot_2016-06-08-14-09-54_zjsx.freearrow.png)

        <!--orientation：箭头方向，默认：左（left）-->
    <!--arrowColor：箭头颜色，默认：黑色-->
    <!--withPole：是否显示横线，默认：不显示-->
    <!--poleRatio：不包含箭头的部分宽度（Gravity横向时）/高度（Gravity为纵向时）占控件（不包含padding）的比例，默认：0.5-->
    <!--poleWidth：横线的长度，默认：整个内容长度-->
    <!--lineStrokeWidth：线的粗细，默认：1dp-->
    <!--arrowThick:箭头的厚度，<0 表示为三角形，默认:0"-->
    <!-- view没有预留Padding值，务必要给padding值，这样不会造成边缘截断 -->
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="10dp"
        android:text="导航箭头" />

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:gravity="center_vertical"
        android:orientation="horizontal">

        <zjsx.freearrow.lib.FreeArrowView
            android:layout_width="50dp"
            android:layout_height="50dp"
            android:layout_margin="10dp"
            android:background="#FF0000"
            android:paddingBottom="10dp"
            android:paddingLeft="15dp"
            android:paddingRight="15dp"
            android:paddingTop="10dp"
            app:arrowColor="#FFF"
            app:lineStrokeWidth="5dp" />

        <zjsx.freearrow.lib.FreeArrowView
            android:layout_width="50dp"
            android:layout_height="50dp"
            android:layout_margin="10dp"
            android:background="#FF0000"
            android:paddingBottom="10dp"
            android:paddingLeft="15dp"
            android:paddingRight="15dp"
            android:paddingTop="10dp"
            app:arrowColor="#FFF"
            app:lineStrokeWidth="3dp" />

        <zjsx.freearrow.lib.FreeArrowView
            android:layout_width="50dp"
            android:layout_height="50dp"
            android:layout_margin="10dp"
            android:background="#FF0000"
            android:paddingBottom="15dp"
            android:paddingLeft="10dp"
            android:paddingRight="10dp"
            android:paddingTop="15dp"
            app:arrowColor="#FFF"
            app:lineStrokeWidth="3dp"
            app:orientation="up" />

        <zjsx.freearrow.lib.FreeArrowView
            android:layout_width="50dp"
            android:layout_height="50dp"
            android:layout_margin="10dp"
            android:background="#FF0000"
            android:paddingBottom="10dp"
            android:paddingLeft="15dp"
            android:paddingRight="15dp"
            android:paddingTop="10dp"
            app:arrowColor="#FFF"
            app:lineStrokeWidth="3dp"
            app:orientation="right" />

        <zjsx.freearrow.lib.FreeArrowView
            android:layout_width="50dp"
            android:layout_height="50dp"
            android:layout_margin="10dp"
            android:background="#FF0000"
            android:paddingBottom="15dp"
            android:paddingLeft="10dp"
            android:paddingRight="10dp"
            android:paddingTop="15dp"
            app:arrowColor="#FFF"
            app:lineStrokeWidth="3dp"
            app:orientation="down" />
    </LinearLayout>

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="10dp"
        android:text="带柄的箭头" />

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:gravity="center_vertical"
        android:orientation="horizontal">

        <zjsx.freearrow.lib.FreeArrowView
            android:layout_width="100dp"
            android:layout_height="50dp"
            android:layout_margin="10dp"
            android:background="#FF0000"
            android:paddingBottom="10dp"
            android:paddingLeft="15dp"
            android:paddingRight="15dp"
            android:paddingTop="10dp"
            app:arrowColor="#FFF"
            app:lineStrokeWidth="3dp"
            app:orientation="left"
            app:withPole="true" />

        <zjsx.freearrow.lib.FreeArrowView
            android:layout_width="50dp"
            android:layout_height="100dp"
            android:layout_margin="10dp"
            android:background="#FF0000"
            android:paddingBottom="15dp"
            android:paddingLeft="10dp"
            android:paddingRight="10dp"
            android:paddingTop="15dp"
            app:arrowColor="#FFF"
            app:lineStrokeWidth="3dp"
            app:orientation="up"
            app:poleRatio="0.5"
            app:withPole="true" />

        <zjsx.freearrow.lib.FreeArrowView
            android:layout_width="100dp"
            android:layout_height="50dp"
            android:layout_margin="10dp"
            android:background="#FF0000"
            android:paddingBottom="10dp"
            android:paddingLeft="15dp"
            android:paddingRight="15dp"
            android:paddingTop="10dp"
            app:arrowColor="#FFF"
            app:lineStrokeWidth="3dp"
            app:orientation="right"
            app:withPole="true" />
    </LinearLayout>

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="10dp"
        android:text="实心箭头" />

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:gravity="center_vertical"
        android:orientation="horizontal">

        <zjsx.freearrow.lib.FreeArrowView
            android:layout_width="100dp"
            android:layout_height="100dp"
            android:layout_margin="10dp"
            android:background="#FF0000"
            android:paddingBottom="10dp"
            android:paddingLeft="15dp"
            android:paddingRight="15dp"
            android:paddingTop="10dp"
            app:arrowColor="#00F"
            app:arrowThick="20dp"
            app:fillArrow="true"
            app:lineStrokeWidth="10dp"
            app:poleRatio="0.5"
            app:poleWidth="-1dp"
            app:withPole="true" />

        <zjsx.freearrow.lib.FreeArrowView
            android:layout_width="100dp"
            android:layout_height="100dp"
            android:layout_margin="10dp"
            android:background="#FF0000"
            android:paddingBottom="10dp"
            android:paddingLeft="15dp"
            android:paddingRight="15dp"
            android:paddingTop="10dp"
            app:arrowColor="#00F"
            app:arrowThick="-1dp"
            app:fillArrow="false"
            app:lineStrokeWidth="3dp"
            app:orientation="down"
            app:poleRatio="0.5"
            app:poleWidth="-1dp"
            app:withPole="true" />

        <zjsx.freearrow.lib.FreeArrowView
            android:layout_width="100dp"
            android:layout_height="100dp"
            android:layout_margin="10dp"
            android:background="#FF0000"
            android:paddingBottom="10dp"
            android:paddingLeft="15dp"
            android:paddingRight="15dp"
            android:paddingTop="10dp"
            app:arrowColor="#00F"
            app:arrowThick="-1dp"
            app:fillArrow="true"
            app:lineStrokeWidth="10dp"
            app:orientation="up"
            app:poleRatio="0.5"
            app:poleWidth="-1dp"
            app:withPole="true" />
    </LinearLayout>

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="10dp"
        android:text="箭头比例" />

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:gravity="center_vertical"
        android:orientation="horizontal">

        <zjsx.freearrow.lib.FreeArrowView
            android:layout_width="0dp"
            android:layout_height="50dp"
            android:layout_margin="10dp"
            android:layout_weight="1"
            android:background="#FF0000"
            android:paddingBottom="20dp"
            android:paddingLeft="15dp"
            android:paddingRight="15dp"
            android:paddingTop="20dp"
            app:arrowColor="#00F"
            app:arrowThick="-1dp"
            app:fillArrow="true"
            app:lineStrokeWidth="3dp"
            app:poleRatio="0.9"
            app:poleWidth="-1dp"
            app:withPole="true" />

        <zjsx.freearrow.lib.FreeArrowView
            android:layout_width="0dp"
            android:layout_height="50dp"
            android:layout_margin="10dp"
            android:layout_weight="1"
            android:background="#FF0000"
            android:paddingBottom="20dp"
            android:paddingLeft="15dp"
            android:paddingRight="15dp"
            android:paddingTop="20dp"
            app:arrowColor="#00F"
            app:lineStrokeWidth="1dp"
            app:poleRatio="0.9"
            app:poleWidth="-1dp"
            app:withPole="true" />
    </LinearLayout>

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="10dp"
        android:text="虚线箭头" />

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:gravity="center_vertical"
        android:orientation="horizontal">

        <zjsx.freearrow.lib.FreeArrowView
            android:layout_width="0dp"
            android:layout_height="50dp"
            android:layout_margin="10dp"
            android:layout_weight="1"
            android:background="#FF0000"
            android:paddingBottom="20dp"
            android:paddingLeft="15dp"
            android:paddingRight="15dp"
            android:paddingTop="20dp"
            app:dashPole="true"
            app:dashWidth="1dp"
            app:dashGap="1dp"
            app:arrowColor="#00F"
            app:arrowThick="-1dp"
            app:lineStrokeWidth="1dp"
            app:poleRatio="0.9"
            app:poleWidth="-1dp"
            app:withPole="true" />

        <zjsx.freearrow.lib.FreeArrowView
            app:orientation="right"
            android:layout_width="0dp"
            android:layout_height="50dp"
            android:layout_margin="10dp"
            android:layout_weight="1"
            android:background="#FF0000"
            android:paddingBottom="20dp"
            android:paddingLeft="15dp"
            android:paddingRight="15dp"
            android:paddingTop="20dp"
            app:arrowColor="#00F"
            app:lineStrokeWidth="1dp"
            app:dashPole="true"
            app:dashWidth="4dp"
            app:dashGap="2dp"
            app:poleRatio="0.9"
            app:poleWidth="-1dp"
            app:withPole="true" />

        <zjsx.freearrow.lib.FreeArrowView
            app:orientation="right"
            android:layout_width="0dp"
            android:layout_height="50dp"
            android:layout_margin="10dp"
            android:layout_weight="1"
            android:background="#FF0000"
            android:paddingBottom="20dp"
            android:paddingLeft="15dp"
            android:paddingRight="15dp"
            android:paddingTop="20dp"
            app:fillArrow="true"
            app:arrowColor="#00F"
            app:lineStrokeWidth="1dp"
            app:dashPole="true"
            app:dashWidth="2dp"
            app:dashGap="4dp"
            app:poleRatio="0.9"
            app:poleWidth="-1dp"
            app:withPole="true" />
    </LinearLayout>
