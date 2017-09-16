
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

# Backbone plugin
import Backbone from 'backbone'
import BackboneAssociations from 'backbone-associations'

## aporia (难点)
ionic 生命周期
 1.http://www.cnblogs.com/zsl123/p/5989214.html
 ionViewLoaded  页面加载完毕触发。该事件发生在页面被创建成 DOM 的时候，且仅仅执行一次。如果页面被缓存（Ionic默认是缓存的）就不会再次触发该事件。该事件中可以放置初始化页面的一些事件
 ionViewWillEnter 即将进入一个页面变成当前激活页面的时候执行的事件。
 ionViewDidEnter 进入了一个页面且变成了当前的激活页面，该事件不管是第一次进入还是缓存后进入都将执行
 ionViewWillLeave 将要离开了该页面之后变成了不是当前激活页面的时候执行的事件
 ionViewDidLeave 在页面完成了离开该页面并变成了不是当前激活页面的时候执行的事件
 ionViewWillUnload 在页面销毁和页面中有元素移除之前执行的事件
 ionViewDidUnload 在页面销毁和页面中有元素移除之后执行的事件

# FAQ


