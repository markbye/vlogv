[![GitHub issues](https://img.shields.io/github/issues/markbye/vlogv.git?color=green&label=vlogv&logo=logo&logoColor=red)](https://github.com/markbye/vlogv.git/issues)

[![GitHub stars](https://img.shields.io/github/stars/markbye/vlogv.git)](https://github.com/markbye/vlogv.git/stargazers)

[![GitHub forks](https://img.shields.io/github/forks/markbye/vlogv.git)](https://github.com/markbye/vlogv.git/network)

### git 添加项目徽章
'''
https://shields.io/
'''

# vlogv
vue log warn log debug
## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### 引入 & use
```
import vLogger from "vlogv";
Vue.use(vLogger, {
  prefix: () => new Date(),
  dev: true,
  shortname: true,
  levels: ["log", "warn", "debug", "error"],
  forceLevels: []
});
PS: 关于shortname，默认是 true，如果不想要别名 那就要用this.$console.log()
// 全局使用
Vue.console.log("hello world");
```
