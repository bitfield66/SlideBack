# SlideBack
一个仿 即刻APP 滑动返回效果的Demo

# 效果
https://user-gold-cdn.xitu.io/2018/8/20/1655691cada3b454?imageslim

# 使用方法：

Step 1. 在你项目的根build.gradle中添加jitpack.io库
````
allprojects {
	repositories {
		...
		maven { url 'https://jitpack.io' }
	}
}
````

Step 2. 添加SlideBack的依赖
````
dependencies {
	implementation 'com.github.ChenTianSaber:SlideBack:v0.6.0'
}
````

Step 3. 将项目中继承的Activity换成SlideBackActivity
````
public class YourActivity extends SlideBackActivity
````

Step 4. 重写slideBackSuccess(当滑动有效时会回调这个方法，可以在这里进行回退操作或其他)
````
@Override
protected void slideBackSuccess() {
   finish();//或者其他
}
````

###### 希望大家能给我Star...
