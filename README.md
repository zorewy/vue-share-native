#vue-share-native版本说明:

##vue分享插件 v1.0.0 主要实现业务功能

##安装

```html
npm install vue-share-native -S
```

##引入分享
```html
 import VueShareNative from '@/components/share'
```
##全局注入
```html
 Vue.use(VueShareNative)
```
##调用分享
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