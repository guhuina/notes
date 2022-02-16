# CSS--clamp函数使用
> clamp() 函数的作用是把一个值限制在一个上限和下限之间，当这个值超过最小值和最大值的范围时，在最小值和最大值之间选择一个值使用。

## 语法
clamp() 函数接收三个用逗号分隔的表达式作为参数，按最小值、首选值、最大值的顺序排列。
```
{
    font-size: clamp(20px, 10%, 40px);
    width: clamp(500px, 50% + 20px, 800px);
}
```
* 当首选值比最小值要小时，则使用最小值。
* 当首选值介于最小值和最大值之间时，用首选值。
* 当首选值比最大值要大时，则使用最大值。

## 兼容性
https://caniuse.com/?search=clamp
从 caniuse 网站可以看出，不支持IE11。

## DEMO 响应式布局for clamp
```
<div class="user">
  <img src="https://picsum.photos/id/64/200/250" alt="user name">
  <h2>Jane Doe</h2>
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum sed ante fringilla, rutrum turpis nec, sagittis massa. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque metus dui, cursus eu hendrerit eget, cursus sed tellus. Mauris congue vestibulum tristique. </p>
</div>
```
```
.user {
  --w:450px;
  --c:(100vw - var(--w));
  
  max-width:500px;
  background:#fff;
  margin:10px auto;
  border-radius:10px;
  overflow:hidden;
  padding:0 20px 0 clamp(20px,var(--c)*1000,180px);
  box-sizing:border-box;
  box-shadow:1px 2px 5px #0005;
  position:relative;
}
.user img {
  position:absolute;
  top:clamp(0px,var(--c)*-1000,10px);
  left:clamp(0px,var(--c)*-1000,20px);
  width:clamp(50px,var(--c)*1000,150px);
  height:clamp(50px,var(--c)*1000,100%);
  border-radius:clamp(0px,var(--c)*-1000,50px);
  object-fit:cover;
  object-position:top;
}
.user h2 {
  margin:20px 0 10px clamp(0px,var(--c)*-1000,70px);
}

body {
  background:pink;
}
```