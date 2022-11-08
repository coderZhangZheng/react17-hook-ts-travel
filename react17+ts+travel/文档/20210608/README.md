**本项目是react+ts技术栈的大型电商平台**
使用create-react-app创建项目
  npx create-react-app my-app
  cd my-app
  npm install
  npm start
使用create-react-app创建基于TypeScript的项目
  npx create-react-app my-app-ts --template typescript
  建议在tsconfig.json中第三行加上"noImplicitAny": false,
  cd my-app-ts
  npm install
  npm start
-----------------------------------
添加/安装项目依赖
  npm install {库名} --save
  或
  yarn add {库名}
删除依赖项目
  npm uninstall package --save
  或
  yarn remove package
升级某个依赖项目
  npm update --save
  或
  yarn upgrade
全局安装某项目依赖(慎用)——因为不同项目可能用到不同版本依赖包
  npm install package -g
  或
  yarn global add package
-----------------------------------
1.如何启动一个React项目？
2.如何启动一个TypeScript版本的React项目？
3.create-react-app是什么？
4.npm与yarn的区别是什么？
5.tsconfig.json有什么用？
6.如何配置TypeScript编译器？
7.npx和npm关系？
  npx是npm的加强版，以create-react-app为例，以往需要先全局安装后创建项目。有了npx之后，可以直接使用一条命令创建my-app项目：
  npx create-react-app my-app
8.package.json中dependencies属性——react-scripts依赖包作用？
  react-scripts是react脚手架的核心包，可以帮助自动构建打包项目，同时帮助我们自动加载babel类似这样的工具。
9.package.json中scripts属性意义？
  使用npm xxx命令执行scripts对象中的配置项时，会自动到./node_modules目录下寻找对应的库
10.使用create-react-app创建基于Typescript的项目时注意点？
  Typescript项目和ES6一样不能被浏览器直接读取，必须转化成ES5，这一代码转化的步骤就叫编译。编译Typescript项目代码必须使用相应的编译器，最常用的有ts-loader,awesome-typescript-loader以及babel-loader。因为使用了create-react-app脚手架，所以默认编译器是babel-loader。
  编译器的配置文件是：tsconfig.json
  强烈建议创建完ts项目后在tsconfig.json中第三行加上
  "noImplicitAny": false,    //不需要显式声明变量的类型any,提高效率
11.如何将已有的react项目修改成支持TS的项目
  1安装ts相关依赖
  npm install --save typescript @types/node @types/react @types/react-dom @types/jest
  2将项目中所有的js和jsx后缀修改为tsx
  3运行npm start后会自动生成tsconfig.json文件
-----------------------------------
1.什么是React?
2.React有什么特点？优势，劣势是什么？
3.什么是JSX？为什么浏览器无法读取JSX？
4.什么是虚拟DOM？
5.什么是组件？
6.state和props有哪些区别？
7.React组件的生命周期有哪些阶段？
-----------------------------------
1.什么是Hooks?
2.什么是纯函数？
3.什么是副作用？
4.有状态和无状态组件的区别？
5.如何跨组件传递数据？
6.HOC是什么意思？
