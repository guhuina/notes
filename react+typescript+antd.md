## typescript config配置文件
```
{
  "compilerOptions": {
    "target": "es5",    //指定ECMAScript的目标版本
    "lib": [
      "dom",
      "dom.iterable",
      "esnext"
    ], //编译过程中需要引入的库文件的列表。
    "allowJs": true, //允许编译javascript文件。
    "skipLibCheck": true, //忽略所有的声明文件（ *.d.ts）的类型检查。
    "esModuleInterop": true,
    "allowSyntheticDefaultImports": true, //允许从没有设置默认导出的模块中默认导入。这并不影响代码的输出，仅为了类型检查。
    "strict": true, //启用所有严格类型检查选项。
    "forceConsistentCasingInFileNames": true,  //禁止对同一个文件的不一致的引用。
    "noFallthroughCasesInSwitch": true, //报告switch语句的fallthrough错误。（即，不允许switch的case语句贯穿）
    "module": "esnext", //指定生成哪个模块系统代码： "None"， "CommonJS"， "AMD"， "System"， "UMD"， "ES6"或 "ES2015"。
    "moduleResolution": "node", //决定如何处理模块。或者是"Node"对于Node.js/io.js，或者是"Classic"
    "resolveJsonModule": true,
    "isolatedModules": true, //将每个文件作为单独的模块（与“ts.transpileModule”类似）。
    "noEmit": true, //不生成输出文件。
    "jsx": "react-jsx" //在 .tsx文件里支持JSX： "React"或 "Preserve"。查看 JSX。
  },
  "include": [
    "src"
  ]
}
```

