### module语法

#### export

1.命名导出（每个模块可包含任意数量）
1.1 导出单个
1.2 导出单个
1.3 导出时重命名

**关键字**：export

2.默认导出（每个模块仅能有一个）

**关键字**：export default

#### import

1.与命名导出对应，需要与导出接口的名称一一对应，并用大括号括起来，也可用as重命名
2.与默认导出对应，不需要使用大括号，直接导入即可
3.导入整个模块，并将模块中所有的导出加载在对象上
**关键字**：import * as xx from 'xx'
4.仅仅执行加载模块，而不导入任何东西
例子：import './profile.js'

#### export和import的复合写法

这种写法也可以重命名接口

例子：
```
export { foo, bar } from 'my_module';

// 可以简单理解为
import { foo, bar } from 'my_module';
export { foo, bar };
```

**注意**：使用复合写法，foo和bar实际上并没有被导入模块，只是相当于转发了两个接口
导致当前模块不能使用foo和bar

参考资料：
[Module语法](https://es6.ruanyifeng.com/?search=%E6%8F%90%E5%8D%87%E6%95%88%E6%9E%9C&x=0&y=0#docs/module)

[export](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Statements/export)

[import](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Statements/import)