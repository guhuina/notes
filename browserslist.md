# browserslist
> 用来指定了项目的目标浏览器的范围

##  browserslist里包含的工具有
* Autoprefixer
* Babel
* postcss-preset-env
* eslint-plugin-compat
* stylelint-no-unsupported-browser-features
* postcss-normalize


## 使用方法
```
{
  "name": "my-react-app",
  "version": "0.1.0",
  "private": true,
  "dependencies": {},
  "scripts": {},
  "eslintConfig": {},
  "browserslist": {
    "production": [
      ">0.2%",
      "not dead",
      "not op_mini all"
    ],
    "development": [
      "last 5 chrome version",
      "last 5 firefox version",
      "last 5 safari version"
    ]
  }
}
```

## 参考链接[https://blog.csdn.net/ap1005233/article/details/101687008](https://blog.csdn.net/ap1005233/article/details/101687008)