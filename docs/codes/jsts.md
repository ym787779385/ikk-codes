# JS/TS

 这是一个动态维护的风格与实践规范。js风格采用```StandardJS```风格，ts风格采用谷歌的ts风格。再此基础上，我们根据自己的业务需求，添加了一些额外的约束。

### 风格

| 优先级 | 权重 | 内容                                                         |
| ------ | ---- | ------------------------------------------------------------ |
|        |      | 优先使用匿名函数，尽量不使用匿名表达式                       |
|        |      | 匿名函数中，如果不需要给参数加括号，则不加括号。例如：```(x) => Math.round(x)```  应该写成 ```x => Math.round(x)``` |
|        |      | 布尔类型的变量都用```is```开头，例如：```isButtonClicked```  |
|        |      | 用动词的过去分词形式```-ed```后缀表示查询一个已经发生的状态。例如：```isAudioPlayed``` |
|        |      | 用动词的现在分词形式```-ing```来表示一个正在进行的状态。例如：```isAudioPlaying``` |
|        |      | 类型或者Class以Pascal命名。例如：```class MyBestClass {}```, ```type MyType = string[]``` |
|        |      | ts/js模块的文件名小写```my-modules.ts```, 但VueJS中的组件，需要使用Pascal命名法。 |


### js规范

| 优先级 | 权重 | 内容                                                         |
| ------ | ---- | ----------------------------------------------------------- |
|        |      | 字面量值创建对象，不能使用保留字作为对象的键值  |
|        |      | 对象方法，对象值简写。对象属性值的简写方式要和声明式的方式分组 |
|        |      | 使用字面量值创建数组，添加元素时使用Push，使用…复制数组 |
|        |      | 使用数组的 map 等方法时，请使用 return 声明，如果是单一声明语句的情况，可省略 return |
|        |      | 使用对象/数组的多个属性时，使用解构赋值 |
|        |      | 不要使用 arguments，可以选择使用 ... |
|        |      | 使用 class，避免直接操作 prototype |
|        |      | 不要使用 iterators |
|        |      | 禁止使用eval(),with(){} |
|        |      | JavaScript的CSS类：如果在Javascript中使用该类，则需要在其前面添加 js- |
|        |      | 字符串解析为数字 ：parseInt()优于Number()或+ |
|        |      | 避免添加到全局命名空间 |
|        |      | 一个函数或类最多使用3个参数。如果需要更多, 使用对象 |

> 参考内容
>
> https://github.com/google/ts-style
>
> https://standardjs.com/