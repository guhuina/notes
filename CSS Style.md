# css style
## 移动端禁止页面下滑

```
html,body{
	overflow: hidden
}
```

## a链接或JavaScript的可点击的元素时，覆盖显示的高亮颜色。
```
*:not(input):not(textarea) {
      user-select: none;
      -webkit-touch-callout: none;
      -webkit-tap-highlight-color: transparent;
    }
```

## 表单轮廓线消失
```
 outline: none;
```


## background-clip 渐变字体
```
-webkit-background-clip: text;
background: linear-gradient(180deg,#fff,#f5222d),#fff;
```