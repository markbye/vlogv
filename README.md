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
