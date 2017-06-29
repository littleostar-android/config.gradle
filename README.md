# config.gradle
config.gradle 统一android 版本

----

----

// 1 定义

// 项目根目录下创建文件config.gradle

```
ext {
    version = [
            compileSdkVersion: 25,
            buildToolsVersion: '25.0.3',
            minSdkVersion    : 15,
            targetSdkVersion : 25
    ]
    dependencies = [
            v4                 : 'com.android.support:support-v4:25.3.1', // v4
            v7                 : 'com.android.support:appcompat-v7:25.3.1', // v7
            design             : 'com.android.support:design:25.3.1', // design
            recyclerview       : 'com.android.support:recyclerview-v7:25.3.1', // recyclerview
            constraint_layout  : 'com.android.support.constraint:constraint-layout:1.0.2',

            junit              : 'junit:junit:4.12', // 单元测试工具

            jsoup              : 'org.jsoup:jsoup:1.10.2', // java爬虫, html解析工具

            // 适配器部分
            base_adapter_helper: 'com.joanzapata.android:base-adapter-helper:1.1.11', // base_adapter_helper
            base_rvadapter     : 'com.zhy:base-rvadapter:3.0.3', // hongyang_recyclerview
            base_adapter       : 'com.zhy:base-adapter:3.0.3', // hongyang_listview
            brvah              : 'com.github.CymChad:BaseRecyclerViewAdapterHelper:2.9.18', // BRVAH

//            nohttp           : 'com.yanzhenjie.nohttp:nohttp:1.1.2',
//            no_okhttp        : 'com.yanzhenjie.nohttp:okhttp:1.1.2',
            okhttp3            : 'com.squareup.okhttp3:okhttp:3.8.0', // 网络请求框架okhttp3
            okhttputils        : 'com.zhy:okhttputils:2.6.2', //
            okgo               : 'com.lzy.net:okgo:3.0.1', // okgo
            async_http         : 'com.loopj.android:android-async-http:1.4.9', // 网络请求框架asynchttp

            greendao           : 'org.greenrobot:greendao:3.2.2', // greendao

            easysp             : 'com.white:easysp:1.0.0', // sharedpreferences 工具类

            glide              : 'com.github.bumptech.glide:glide:4.0.0-RC0', // 图片加载框架glide

            gson               : 'com.google.code.gson:gson:2.8.0',   // json解析 gson
            fastjson           : 'com.alibaba:fastjson:1.2.32', // json解析 fastjson

            rxgalleryfinal     : 'cn.finalteam.rxgalleryfinal:library:1.0.7', // 图片选择器
            galleryfinal       : 'cn.finalteam:galleryfinal:1.4.8.7', // 图片选择器

            andpermission      : 'com.yanzhenjie:permission:1.0.8' // andpermission 运行时权限
    ]
}

/*
    主流图片加载框架
    compile 'com.squareup.picasso:picasso:2.5.2'
    compile 'com.facebook.fresco:fresco:0.12.0'
    compile 'com.github.bumptech.glide:glide:3.7.0'
    compile 'com.nostra13.universalimageloader:universal-image-loader:1.9.5'
 */
```

----

// 2 导入 

// 项目级别build.gradle引入config.gradle

//apply from: 'config.gradle'

----

// 3 使用

// 

//def conf = rootProject.ext.android

//def libs = rootProject.ext.dependencies

//compileSdkVersion conf.compileSdkVersion

//buildToolsVersion conf.buildToolsVersion

//minSdkVersion conf.minSdkVersion

//targetSdkVersion conf.targetSdkVersion


----
    Copyright (C) 2017 haomengjie

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

         http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

