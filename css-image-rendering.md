# css 缩小图片后，图片变模糊的解决办法
```
img{
	image-rendering: -moz-crisp-edges;
	image-rendering: -o-crisp-edges;
	image-rendering: -webkit-optimize-contrast;
    image-rendering: crisp-edges;
    -ms-interpolation-mode: nearest-neighbor;
    
}
```