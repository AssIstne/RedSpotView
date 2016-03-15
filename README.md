# RedSpotView
实现便捷地在View上增加小红点.

# 引用方法
依赖
```xml
repositories {
    jcenter()
}

compile 'com.assistne.android:red-spot-view:1.0.1'
```

# 使用方法
```xml
<com.assistne.android.RedSpotView
    android:layout_width="100dp"
    android:layout_height="100dp"
    app:spot_marginRight="16dp"
    app:spot_gravity="left"
    app:spotText="99"
    app:spotColor="@android:color/black"
    app:spotTextSize="12sp"
    app:spotTextColor="@android:color/holo_blue_light"
    app:spotDiameter="30dp">
    <ImageView
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:alpha="0.7"
        android:background="@android:color/holo_blue_light"/>
</com.assistne.android.RedSpotView>
```

> `RedSpotView`实质是一个`RelativeLayout`, 因此你可以使用任意`RelativeLayout`的属性.
不要使用`wrap_content`指定`RedSpotView`的大小.

可以使用的属性包括:

1. `spot_marginLeft`:圆点左侧外边距
2. `spot_marginTop`:圆点顶部外边距
3. `spot_marginRight`:圆点右侧外边距
4. `spot_marginBottom`:圆点底部外边距
5. `spotText`:原点中心文本
6. `spotTextColor`:文本颜色, 默认为白色
7. `spotTextSize`:文本大小, 默认为10sp
8. `spotDiameter`:圆点直径, 默认为16dp
9. `spot_gravity`:圆点位于`RedSpotView`的相对位置, 默认为右上方, 允许值为`left|right|top|bottom`
10. `spotColor`:圆点颜色, 默认为红色
