# 获取本人信息

## url http://tst.candy.one/api/user/authorization-user-info

## 请求方式: Get



### 参数列表
| 参数名称         | 参数类型  | 是否必填 | 参数说明 |
| ---             | ----    | ----    | ----   |
| token          | String     | 是   | 授权成功获得的token |



## 响应

**同步返回**

```javascript
{
    "code":1,
    "data":{
        "avatar":"candy/dync/2941922_1541064461852_0",
        "nick_name":"大漠斜阳西风烈酒",
        "openId":"1fea115e7e39432a20e0b9be46700f72"
    }
}
```
### 返回值
| 参数名称         | 返回值类型  | 说明 |
| ---            | ----     | ----   |
| code          | int     | 1为成功，0为失败
| avatar          | String     | 用户头像url|
| nick_name          | String     | 用户昵称|
| openId          | String     | 用户在第三方平台的open id|



