涉及工具：
```create-react-app```(自行搭建环境也可),
[lerna](https://www.lernajs.cn/)，
```babel```，
```typescript```，
```prettier```,
```yorkie```
服务端工具 [verdaccio](https://verdaccio.org/zh-cn/docs/installation/)

## 一、项目架构

```
my-component-app
├── README.md
├── node_modules
├── package.json
├── .gitignore
├── .prettierignore
├── copy-files.js            //移动各个包下的package.json，.d.ts产物到package下
├── .prettierrc              //commit 格式化代码的格式配置
├── build.js                 //babel 编译代码文件
├── babel.config.js          
├── updatePackage.js         //发包之后同步源码中的包版本号
├── tsconfig.build.json      //生产环境下的tsconfig
├── tsconfig.json
├── lerna.json
├── dist                     //tsc 生成.d.ts的产物
├── packages                 //babel 编译后的产物
├── public
│   ├── favicon.ico
│   ├── index.html
└── src
    ├── giggle-ui
    │   ├── src
        │   ├── index.ts
        │   ├── button.tsx
    │   ├── package.json
    │   ├── README.md
    │   ├── tsconfig.json
    ├── giggle-utils
    ├── giggle-hooks
    ├── App.css
    ├── App.tsx
    ├── index.css
    ├── index.tsx
    └── react-app-env.d.ts
    
```


 