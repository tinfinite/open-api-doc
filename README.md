# 开放平台接口文档

## oauth2授权
### 概要介绍
  授权部分采用业界主流的oauth2协议授权码模式，具体概念介绍可以参考[oauth2介绍](http://www.ruanyifeng.com/blog/2014/05/oauth_2_0.html)  
### 第三方对接步骤
  下面以postman为例，介绍第三方对接我方授权平台的步骤。  
  
  1.选择postman的Authorization的选项，type选择Oauth 2.0,点击Get New Access Token![postman1](myimage/postman1.jpg )  
  2.在新窗口中填入各个选项，点击request token![postman2](myimage/postman2.jpg )  
  3.输入在我方平台已经注册的手机号密码，点击登录![postman3](myimage/postman3.jpg )  
  4.跳转到授权确认页面，点击授权![postman4](myimage/postman4.jpg )  
  5.跳转到显示token页面，授权过程结束![postman5](myimage/postman5.jpg)  

  
### 标题2
* 1、因为是纯文本，所以只要支持Markdown的地方都能获得一样的编辑效果，[百度](http://baidu.com)，可以让作者摆脱排版的困扰，专心写作,**加粗文字**。  
* 2、操作简单。比如:WYSIWYG编辑时标记个标题，先选中内容，再点击导航栏的标题按钮，选择几级标题。要三个步骤。而Markdown只需要在标题内容前加#即可
### 标题2
* [oauth授权](oauth2.md)
* [根据token获取用户信息](user_info.md)
### 标题2
姓名|技能|排行
--|:--:|--:
刘备|哭|大哥
关羽|打|二哥
张飞|骂|三弟

### 代码
```
@Test
    public void testGetToken(){
        String url="http://oauth-tst.candy.one/users/info?access_token=0ecee58e-a9a5-4f02-b4e7-d92858842b2b";
        String ret=doGet(url);
        System.out.println(ret);

    }
```

### 标题2
  正文优点： myimage/WechatIMG51.jpeg   
* 1、因为是纯文本，所以只要支持Markdown的地方都能获得一样的编辑效果，可以让作者摆脱排版的困扰，专心写作。  
![大草原](myimage/WechatIMG51.jpeg "大草原")
* 2、操作简单。比如:WYSIWYG编辑时标记个标题，先选中内容，再点击导航栏的标题按钮，选择几级标题。要三个步骤。而Markdown只需要在标题内容前加#即可


