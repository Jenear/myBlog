# Virtual DOM

## 1:什么是Virtual DOM
Virtual DOM 是一种编程概念：UI以一种思想化的，或者说“虚拟的”表现形式被保存于内存中，并通过ReactDOM等类库使之与“真实的”DOM同步，这一过程叫做reconciliation（协调）

这种方式赋予了React声明式的API：告诉React希望让UI是什么状态，React就确保DOM匹配该状态（可以参考函数式编程中的命令式去理解）。这使我们在运用react开发的时候可以从属性操作、事件处理和手动DOM更新这些在构建应用程序时必要的操作中释放出来。

与其将“Virtual DOM”视为一种技术，不是说它是一种模式，人们提到它的时候是要表达不同的东西。
在React的世界里，"Virtual DOM"通常与react元素关联在一起，它们都是代表了用户界面的对象。
React也使用[fibers](https://github.com/acdlite/react-fiber-architecture)这个内部对象来存放组件数的附加信息，也是"Virtual DOM"的一部分。

## 2：Shadow DOM 和Virtual DOM是一回事吗？
答案是否定的，他们不一样。
Shadow DOM是一种浏览器技术，主要用于在web组件封装变量和css。
而Virtual DOM则是一种由JavaScript类库基于浏览器API实现的概念。


