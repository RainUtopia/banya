

# 瓣呀，一个基于豆瓣api模仿网易云音乐的开源app
----

* 首页分为三大模块，包括：电影、看书、音乐。而电影模块又包括最近热门电影、TOP250；看书模块包括综合、文学、流行、文化、生活五个部分；音乐模块包括流行、经典、韩系、欧美四个模块。

* 抽屉界面的实现是使用DrawerLayout和NavigationView实现，使用的icon来自[material design icon](https://design.google.com/icons/index.html)。

* 首页界面风格采用Material Design设计规范，使用了CoordinatorLayout和viewpager配合，使用behavior属性对toolbar的显示和隐藏进行了控制，tablayout和viewpager配合，整体界面模仿了网易云音乐。

* 详情界面模仿了豆瓣app的详情界面，包括了电影详情、音乐详情、书籍详情，另外使用了webview 对详情页面和导演、演员、作者歌手的个人信息进行了展示。

* 项目整体采用mvp+rxjava+retrofit 框架，用butterknif注解，使用glide进行图片展示，另外使用了java 8 新特性，拉姆达表达式，安卓原生并不支持，需要导插件。

* 对okhttpClient进行了缓存配置，然而豆瓣API并对Cache-Control的设置为no-cache，所以目前没有缓存，需要自己实现，后面会花时间用Realm去实现。



## ScreenShot
----

<a href="art/00.png"><img src="art/00.png" width="40%"/></a> <a href="art/01.png"><img src="art/01.png" width="40%"/></a>
<a href="art/02.png"><img src="art/02.png" width="40%"/></a> <a href="art/03.png"><img src="art/03.png" width="40%"/></a>
<a href="art/04.png"><img src="art/04.png" width="40%"/></a> <a href="art/05.png"><img src="art/05.png" width="40%"/></a>
<a href="art/06.png"><img src="art/06.png" width="40%"/></a> <a href="art/07.png"><img src="art/07.png" width="40%"/></a>
<a href="art/003.png"><img src="art/003.png" width="40%"/></a> <a href="art/004.png"><img src="art/004.png" width="40%"/></a>
<a href="art/08.png"><img src="art/08.png" width="40%"/></a> <a href="art/09.png"><img src="art/09.png" width="40%"/></a>
<a href="art/10.png"><img src="art/10.png" width="40%"/></a> <a href="art/11.png"><img src="art/11.png" width="40%"/></a>
<a href="art/12.png"><img src="art/12.png" width="40%"/></a> <a href="art/13.png"><img src="art/13.png" width="40%"/></a>
<a href="art/14.png"><img src="art/14.png" width="40%"/></a>

## api
----
app所以的api都来自[豆瓣Api V2（测试版）](https://developers.douban.com/wiki/?title=api_v2);一切数据都归豆瓣所有。

## Statement
----
该项目仅供交流学习使用，如果该项目有侵犯版权问题，或被告知需停止共享与使用，本人会及时删除此页面与整个项目。

## 感谢
----

* [RXJava](https://github.com/ReactiveX/RxJava)
* [RxAndroid](https://github.com/ReactiveX/RxAndroid)
* [okhttp](https://github.com/square/okhttp)
* [retrofit](https://github.com/square/retrofit)
* [butterknif](https://github.com/JakeWharton/butterknife)
* [glide](https://github.com/bumptech/glide)


## 关于我
---
一个在深圳的安卓开发者，对技术有着强烈的追求，目前在学习Javascript，希望认识一些志同道合的朋友。
 
## 联系我:
----
 - Email:124746406@qq.com
 - jianshu: [jianshu](http://www.jianshu.com/users/f2550db5eca3/latest_articles)
 - Blog : [csdn blog](http://blog.csdn.net/forezp)
 - GitHub: [Forezp](https://github.com/forezp)
 
##  License
----
Copyright 2016 Forezp

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.


