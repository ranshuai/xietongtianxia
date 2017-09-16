
# 相关技术

## ionic@v3.10 & angular4 & typeScript

>1. http://ionicframework.com/docs/intro/installation/
>2. https://angular.cn/docs
>3. https://www.tslang.cn/docs/home.html
## 页面访问地址

## 线上地址

## 开发目录结构

~~~
src 存放原始文件
├── app 
│   ├── app.module.ts ------------------------------APP 的入口文件
│   └── app.html ------------------------------ 主模版文件
│   
├── assets  ------------------------------图片资源&字体库
│   ├── test1.png
│   ├── test2.png
│   └── test3.png
│
├── components ------------------------------ 定义的组件文件
│   ├── components.module.ts ------------------------------ 组件的集合
│   └── goods-img ------------------------------ 一个组件（ts,html.scss）
│       ├── goods-img.html
│       ├── goods-img.ts
│       └── goods-img.scss
│        
├── directives ------------------------------ 定义的指令文件
│   └── ng-enter.ts ------------------------------ 自定义指令
│
├── lib ------------------------------ 引入的第三方插件
│ 
├── pipes ------------------------------ 定义管道的文件
│   ├── currency ------------------------------ 金额转换
│
├── pages ------------------------------ 关于业务的文件
│   ├──change-roles ------------------------------ 切换身份
│   ├──store ------------------------------ 店铺角色
│   ├──user ------------------------------ 消费者
│   ├── 物流人
│
└── providers --------------------------- 服务
~~~

# 初始化依赖

```shell
npm install
```

# 开发
ionic serve

# 打包
ionic cordova build android --prod

# 发布
* git push origin develop 

# 域名地址
    prod: {
      bl: 'https://b.snsall.com/',
      lg: 'https://l.snsall.com/',
      org: 'https://o.snsall.com/'
    },
    //测试环境
    test: {
      bl: 'https://t.b.snsall.com/',
      lg: 'https://t.l.snsall.com/',
      org: 'https://t.o.snsall.com/'
    },
    //开发环境
    dev: {
      bl:'https://d.b.snsall.com/',  //'http://192.168.1.24:8011/',
      lg: 'https://d.l.snsall.com/', //'http://192.168.1.24:8012/',
      org:'https://d.o.snsall.com/'  //'http://192.168.1.24:8502/'
    }

#Backbone plugin
import Backbone from 'backbone';
import BackboneAssociations from 'backbone-associations';

# FAQ


