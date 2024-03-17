# H5强制发送跨域请求无需CORS配置

分享一个无需服务器配置CORS，在手机上向任意网页发送跨域请求，并携带登录态，可定制任意请求头的方法。

请注意，此特性在[跨时空1.0.28](https://kainy.cn/app/?f=gh_mcb)版本实现，该版本已在AppStore和GooglePlay 应用商店发布。

下面演示用部署在自己的服务器网页（后面称为测试页）： https://kainy.cn/app/pages/test-CORS.html?f=gh_mcb ，发送携带登录信息（cookie）的请求道饿了么的接口。该接口的作用是返回当前登录用户的ID。

----

在普通浏览器中，点击发送请求，可以看到受到了CORS限制

<img src="https://raw.githubusercontent.com/frontender/Mobile-CORS-browser/main/IMG_8143.PNG" style="width:20%;"/>


----

在跨时空浏览器中访问，请求得到了回应，由于未登录，返回的客户ID为 0


<img src="https://raw.githubusercontent.com/frontender/Mobile-CORS-browser/main/IMG_8144.PNG" style="width:20%;"/>

----


点击右上方的“登录态获取”链接，跳转饿了么登录页面，完成登录。

<img src="https://raw.githubusercontent.com/frontender/Mobile-CORS-browser/main/IMG_8145.PNG" style="width:20%;"/>

----

回到测试页，这时再点击发送请求，可以看到服务器返回了我的用户ID

<img src="https://raw.githubusercontent.com/frontender/Mobile-CORS-browser/main/IMG_8146.PNG" style="width:20%;"/>


----

带cookie的跨域请求，可以用于web安全测试、抢红包任务、打卡任务等流程优化，提高工作效率，实乃开发者杀人放火，居家旅行之必备良器。

微信扫码查看解说视频：

<img src="https://raw.githubusercontent.com/frontender/Mobile-CORS-browser/main/image.png" style="width:20%;"/>
