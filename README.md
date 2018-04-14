#vue-share-native开发背景:
因公司业务需要在web实现分享
在普通浏览器不能使用微信分享功能

UC和QQ浏览器因浏览器有分享接口可以调用

在微信内置浏览器 需要微信授权才可以调用 微信的分享接口
所以 我们把微信分享改成了弹窗 引导用户去下载APP

APP的WebView提供了了方法 我们进行交互 当我们在APP中点击分享时
APP提供的方法执行会调用原生的分享

故而写此插件
#vue-share-native版本说明:

#vue分享插件 v1.0.0 主要实现业务功能

#安装

```javascript
npm install vue-share-native -S
```

##引入分享
```javascript
 import VueShareNative from '@/components/share'
```
#全局注入
```javascript
 Vue.use(VueShareNative)
```
#调用分享
```html
 <div class="share" @click="$share"
         data-title="分享弹窗标题"
         data-subtitle="分享弹窗副标题"
         data-share-title= "zore测试分享"
         data-share-url= "http://zore.wang"
         data-share-pic= "https://www.zore.wang/static/images/vueshare/lovely-girl.jpg"
         data-share-des= "前端开发、web前端开发、HTML5、JavaScript/Vue"
         data-app-from= "来自zore分享组件"
         data-share-type= "1"
         data-popup-title= "下载弹窗标题"
         data-app-url= "app下载地址">
      显示分享
</div>
```
##Demo

* [Demo](https://zore.wang/VueUtils/VueShareNative/) 