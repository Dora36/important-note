# Coding Style

> *不管有多少人共同参与同一项目，一定要确保每一行代码都像是同一个人编写的。*

## 编辑器 (VS Code)

1. Tab 使用两个空格。

2. 请牢记 `Shift + Option + F`。

## 文件名

1. 文件名必须全部为小写，并且可以包含下划线 `_` 或短横线 `-`，但不能包含其他标点符号。建议使用短横线 `-`。

## HTML

1. 标签、属性名应全部 **小写**，不要大写。

2. 属性值全部使用 `""` 双引号，不要使用 `''` 单引号。

3. `class` 属性值一律使用 **小写英文字母** 和 **-** 命名。

4. HTML 的属性不要换行。

5. 嵌套元素应正常缩进（用两个空格）。

## CSS

1. 将左花括号与选择器放在同一行，并且左花括号与选择器间添加一个空格。

2. 冒号与属性值之间添加一个空格。

3. 逗号和符号之后添加一个空格。

4. 每个属性与值结尾都要使用分号。

5. 右花括号放在新的一行。

## JS

1. 通常运算符 `=`、`+`、`-`、`*`、`/`、`{`、`}` 等前后需要添加空格；`,` 之后需要添加空格；`()` 和 `[]` 内不需要添加空格。

2. js 中字符串使用 **' '** 单引号；有变量或需要换行的时候，使用 **``** 反单引号。

### 变量

1. 变量命名：js 中的变量和函数一律使用 **小驼峰命名法**；

2. 变量声明：不要用 `var`，尽量都用 `let`。用 `const` 声明的常量，常量名最好都大写，`import` 除外。

3. 语义化命名：变量名要有含义。通过含义就能知道变量的作用。名字是给人看的，不是给电脑看的。

4. `import` 引入模块命名一律使用 **大驼峰命名法**，首字母大写。

### 语法

1. 不要再 `Array` 上使用 `for-in` 循环。`for-in` 循环只用于 `object/map/hash` 的遍历, 对 `Array` 用 `for-in` 循环有时会出错. 因为它并不是从 `0` 到 `length - 1` 进行遍历, 而是所有出现在对象及其原型链的键值。

2. 跨行语法中，操作符始终写在前一行, 以免分号的隐式插入产生预想不到的问题。

3. 使用三元操作符代替部分 `if` 条件判断语句。

4. `for` 循环中首先缓存数组长度，避免每次循环重新计算。`let len = arr.length; for(let i = 0; i < len; i++){}`。

5. 如果没有特殊说明，`class` 类有默认的构造方法。不用特意写一个空的构造函数或只是代表父类的构造函数。

6. 在注释前加上 `FIXME:` 或 `TODO:` 前缀， 这有助于其他开发人员快速理解你指出的问题， 或者您建议的问题的解决方案。

7. 默认导出（`export default`）一个函数时，函数名、文件名统一。

[*参考链接 - Airbnb JavaScript Style Guide*](https://github.com/airbnb/javascript)