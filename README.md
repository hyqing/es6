es6示例1

支持module的配置

1.安装babel相关依赖
``` 
npm install --save babel-core
npm install --save babel-preset-env或者es2015
npm install babel-cli -g
```

2.在根目录创建.babelrc文件，内容如下
```
{
    "presets": [
     "env"或者"es2015"
    ],
    "plugins": []
}
```

3.运行命令执行js

```
babel-node xxx.js
```

参考资料：
[安装babel和配置、执行](https://blog.csdn.net/wushichao0325/article/details/85262063)