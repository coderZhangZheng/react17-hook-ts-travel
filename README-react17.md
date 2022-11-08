# React17 + React-Router-v6

## React16->18 的变化

```
React16->17的变化
  v16之前痛不欲生，大版本不兼容，更新非常快
  v16.3-8之间的小版本增加了很多新特性(生命周期，Hooks...)
  v17中删除document上的事件委托改成根DOM容器
React17->18的变化
  v17之后都是渐进更新，vue2后也是一样
  v18新功能：并发渲染(全自动)，新Suspense组件
  v18新特性：startTransition
  破坏性改变：https://zh-hans.reactjs.org/blog/2020/10/20/react-v17.html
```

## React 源码核心概念

```
reconciliation 协调
rendering 渲染
React Components
    函数式组件
    类组件
React elements
    const App = () => {
      return (
        <div>App component</div>
      )
    }
    console.log(App())   // Object, jsx => React.createElement()
Component instance
```
