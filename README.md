# Layout_all_three




## 实验二Android布局

1.线性布局



截图如下：
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190318193220862.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1NhbW11cmFtYXQ=,size_16,color_FFFFFF,t_70)





源代码如下：
```
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:orientation="vertical"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#000000">
    <LinearLayout
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textColor="#7D7D7D"
            android:text="one,one"
            android:textSize="10dp"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textColor="#7D7D7D"
            android:text="one,two"
            android:textSize="10dp"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textColor="#7D7D7D"
            android:text="one,three"
            android:textSize="10dp"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textColor="#7D7D7D"
            android:text="one,four"
            android:textSize="10dp"/>
    </LinearLayout>
    <LinearLayout
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textColor="#7D7D7D"
            android:text="two,one"
            android:textSize="10dp"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textColor="#7D7D7D"
            android:text="two,two"
            android:textSize="10dp"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textColor="#7D7D7D"
            android:text="two,three"
            android:textSize="10dp"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textColor="#7D7D7D"
            android:text="two,four"
            android:textSize="10dp"/>
    </LinearLayout>
    <LinearLayout
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textColor="#7D7D7D"
            android:text="three,one"
            android:textSize="10dp"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textColor="#7D7D7D"
            android:text="three,two"
            android:textSize="10dp"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textColor="#7D7D7D"
            android:text="one,three"
            android:textSize="10dp"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textColor="#7D7D7D"
            android:text="three,four"
            android:textSize="10dp"/>
    </LinearLayout>
    <LinearLayout
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="horizontal">
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textColor="#7D7D7D"
            android:text="four,one"
            android:textSize="10dp"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textColor="#7D7D7D"
            android:text="four,two"
            android:textSize="10dp"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textColor="#7D7D7D"
            android:text="four,three"
            android:textSize="10dp"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textColor="#7D7D7D"
            android:text="four,four"
            android:textSize="10dp"/>
    </LinearLayout>
</LinearLayout>
```
2.实现布局界面




截图如下：
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190318193731316.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1NhbW11cmFtYXQ=,size_16,color_FFFFFF,t_70)




源代码如下：
```
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:minHeight="0dp"
    android:background="#000000"
    android:orientation="horizontal">
    <Button
        android:id="@+id/one"
        android:layout_width="80dp"
        android:layout_height="wrap_content"
        android:background="#FF0000"
        android:layout_marginLeft="3dp"
        android:textColor="#000000"
        android:text="Red" />

    <Button
        android:id="@+id/two"
        android:layout_width="100dp"
        android:layout_height="wrap_content"
        android:layout_marginLeft="145dp"
        android:background="#EE9A00"
        android:textColor="#000000"
        android:text="orange" />

    <Button
        android:id="@+id/three"
        android:layout_width="80dp"
        android:layout_height="wrap_content"
        android:layout_marginLeft="302dp"
        android:background="#FFF000"
        android:textColor="#000000"
        android:text="yellow" />

    <Button
        android:id="@+id/four"
        android:layout_width="80dp"
        android:layout_height="wrap_content"
        android:layout_marginLeft="70dp"
        android:layout_marginTop="100dp"
        android:background="#7FFF00"
        android:textColor="#000000"
        android:text="green" />

    <Button
        android:id="@+id/five"
        android:layout_width="80dp"
        android:layout_height="wrap_content"
        android:layout_marginLeft="158dp"
        android:layout_marginTop="100dp"
        android:background="#0000EE"
        android:textColor="#000000"
        android:text="blue" />

    <Button
        android:id="@+id/six"
        android:layout_width="80dp"
        android:layout_height="wrap_content"
        android:layout_marginLeft="246dp"
        android:layout_marginTop="100dp"
        android:background="#4B0082"
        android:textColor="#000000"
        android:text="indigo" />

    <Button
        android:id="@+id/seven"


android:layout_width="match_parent"
        android:layout_height="80dp"
        android:layout_alignParentLeft="true"
        android:layout_marginTop="200dp"
        android:background="#DDA0DD"
        android:textColor="#000000"
        android:text="violef" />
</RelativeLayout>
```
3.表格布局



截图如下：
![在这里插入图片描述](https://img-blog.csdnimg.cn/20190318193951842.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L1NhbW11cmFtYXQ=,size_16,color_FFFFFF,t_70)




源代码如下：
```
<?xml version="1.0" encoding="utf-8"?>
<TableLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:stretchColumns="1"
    android:background="#000000">

    <TableRow>
        <TextView
            android:layout_column="1"
            android:text="Open..."
            android:padding="3dip"
            android:textColor="#ffffff"/>
        <TextView
            android:text="Ctrl-O"
            android:gravity="right"
            android:padding="3dip"
            android:textColor="#ffffff"/>

    </TableRow>

    <TableRow>
        <TextView
            android:layout_column="1"
            android:text="Save..."
            android:padding="3dip"
            android:textColor="#ffffff"/>
        <TextView
            android:text="Ctrl-S"
            android:gravity="right"
            android:padding="3dip"
            android:textColor="#ffffff"/>
    </TableRow>

    <TableRow>
        <TextView
            android:layout_column="1"
            android:text="Save As..."
            android:padding="3dip"
            android:textColor="#ffffff"/>
        <TextView
            android:text="Ctrl-Shift-S"
            android:gravity="right"
            android:padding="3dip"
            android:textColor="#ffffff"/>
    </TableRow>

    <View
        android:layout_height="2dip"
        android:background="#ffffff"/>
    <TableRow>
        <TextView
            android:text="X"
            android:textColor="#ffffff"
            android:padding="3dip"/>
        <TextView
            android:text="Import..."
            android:textColor="#ffffff"
            android:padding="3dip"/>
    </TableRow>
    <TableRow>
        <TextView
            android:text="X"
            android:textColor="#ffffff"
            android:padding="3dip"/>
        <TextView
            android:text="Emport..."
            android:textColor="#ffffff"
            android:padding="3dip"/>
        <TextView
            android:text="Ctrl-E"
            android:gravity="right"
            android:textColor="#ffffff"
            android:padding="3dip"/>
    </TableRow>
    <View
        android:layout_height="2dip"

        android:background="#ffffff"/>
    <TableRow>
        <TextView
            android:layout_column="1"
            android:textColor="#ffffff"
            android:text="Quit"
            android:padding="3dip"/>
    </TableRow>
</TableLayout>

```

