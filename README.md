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
            v4               : 'com.android.support:support-v4:25.3.1', // v4
            v7               : 'com.android.support:appcompat-v7:25.3.1', // v7
            constraint_layout: 'com.android.support.constraint:constraint-layout:1.0.2',

            junit            : 'junit:junit:4.12' // 单元测试工具
	]
}
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

