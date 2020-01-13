# test

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).


//--修改elment-ui 源码流程
 //  packages文件夹中存放的就是各种组件源码，可以根据需要去进行修改，修改完成后重新执行npm run dist就会重新打包，覆盖lib文件夹
 
//  /packages/theme-chaik下是elementUI各个组件的样式文件

// 源码中样式采用sass进行预编译，所以如果要修改源码样式就需要在src文件夹下找到相应的样式进行修改，修改完成后在theme-chalk文件夹下， npm install安装依赖，安装完后使 // 用npm run build对样式进行编译和打包，（样式打包使用的是gulp工具），打包后文件会覆盖theme-chalk下的lib文件夹。

//  修改完逻辑和样式，并对样式文件进行重打包后，返回根目录下npm run dist即可打包生成最后的文件。完成后将根目录下lib文件夹替换自己项目    中/node_module/element-ui/lib即可。

