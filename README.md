vue-scooter is a lightweight vue file loader for browser
## 警告！实验阶段
该vue-scooter设计用于兼容性要求较低的前端项目 (如企业内部系统), 在浏览器端实现vue单文件组件解析, 快速启动模块化的静态页面开发, 配套轻量化部署, 支持在生产环境运行, 当前处于实验阶段

## 浏览器兼容性要求
Chrome 63+  
Firefox 67+  
Edge 79+  
Safari 11.1+

## Todo list
```
[√] 加载vue入口文件  
[√] vue单文件组件解析
    [√] 分离template/script/style
    [√] 处理script
        [√] import js
            [√] 相对路径替换
        [√] import vue (子组件)
            [√] 相对路径替换    
            [√] 防止重复加载
            [√] 遍历
            [√] 递归解析
    [√] 处理template
        [√] 相对路径替换
    [√] style解析
        [√] css嵌套
        [√] 变量（原生var测试）
        [√] 资源引用相对路径替换
        [√] scoped
    [√] vue-router懒加载测试
    [√] npm三方库引用 (import cdn文件)
    [√] 支持静态资源前缀配置
[x] 加载异常处理
[-] 开发模式热重载支持
    [x] 样式热重载
    [√] vue组件热重载
[-] 配套轻量部署方式
    [√] 部署文件版本控制
    [x] 静态资源前缀配置
    [x] vue切换生产版本
...
```
## Dependencies
[stylis](https://github.com/thysultan/stylis.js)  
[vue-hot-reload-api](https://github.com/vuejs/vue-hot-reload-api)  

## License
[MIT](http://opensource.org/licenses/MIT)
