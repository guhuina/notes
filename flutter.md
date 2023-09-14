# flutter
> GPU渲染 120fps google公司出品和推广
> 组件的生态环境 https://github.com/Solido/awesome-flutter
> 

## 安装
打开.bash_profile并编辑
```
open .bash_profile       //      ～/.zshrc    source ～/.bash_profile

export PATH=/Users/hb/flutter/bin:$PATH
export PUB_HOSTED_URL=https://mirrors.tuna.tsinghua.edu.cn/dart-pub
export FLUTTER_STORAGE_BASE_URL=https://mirrors.tuna.tsinghua.edu.cn/flutter

```

[安装][https://www.jianshu.com/p/bb9b4bf13a48]
[学习][https://flutterchina.club/setup-macos/]


##使用外部包(package
 pubspec.yaml文件管理Flutter应用程序的assets(资源，如图片、package等)
```
flutter packages get  //安装依赖包
import 'package:flutter/material.dart';
import 'package:english_words/english_words.dart';  //引入 english_words,

```


## flutter 命令
```
flutter doctor //检查我们flutter安装是否正确
flutter upgrade //升级Flutter SDK和依赖包
flutter packages get //获取项目所有的依赖包。
flutter packages upgrade //获取项目所有依赖包的最新版本。
flutter run
flutter create demo //创建一个flutter项目		/lib/main.dart 入口文件

```

## Material APP [https://material.io/]
* StatelessWidget 静态组件
```
	import 'package:flutter/material.dart';
	void main() => runApp(new MyApp());

    class MyApp extends StatelessWidget {
      @override
      Widget build(BuildContext context) {
        return new MaterialApp(
          title: 'Welcome to Flutter',
          home: new Scaffold(
            appBar: new AppBar(
              title: new Text('Welcome to Flutter'),
            ),
            body: new Center(
              child: new Text('Hello World'),
            ),
          ),
        );
      }
    }
```
* StatefulWidget   动态组件
   * Scaffold  //它提供了默认的导航栏、标题和包含主屏幕widget树的body属性
   
   ### Pixel density 
   	* [https://material.io/design/layout/pixel-density.html#pixel-density]
   	* [https://blog.csdn.net/sinat_17775997/article/details/95375676]
   
