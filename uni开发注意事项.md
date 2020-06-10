###### 1.scroll-view中使用flex布局会失效，应当在scroll-view中嵌套一层元素再使用flex布局

```html
<!--职位推荐导航-->
    <view class="index-position-recommend">
      <scroll-view scroll-x="true" class="recommend-list-container">
        <view class="recommend-list">
          <view class="recommend-item" v-for ="(item,index) in recommendList" :key="index">
            {{item}}
          </view>
        </view>
      </scroll-view>
    </view>
    <!--职位推荐导航 -end- -->
```

###### 2.清除scroll-view滚动条

```css
//隐藏scroll-view滚动条
::-webkit-scrollbar {
	width: 0;
	height: 0;
	color: transparent;
}
```

3.阻止穿透(弹出层中无scroll-view),方法使用空实现

```html
<view @touchmove.stop.prevent="moveHandle">
</view>
```

```js
  moveHandle(){
    
  }
```

4.阻止有scroll-view的弹出层穿透问题，弹出层弹出时，将页面高度限制为视口高度，弹出层关闭时解除限制



