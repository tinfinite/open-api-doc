# 开放平台 接口文档

## 标题1
### 标题2
  正文，，，，，，，优点：  
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


