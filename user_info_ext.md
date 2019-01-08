# 获取用户信息

## url http://tst.candy.one/api/user/1.0.0/authorization-user-info

## 请求方式: Get

### 头列表
| 参数名称         | 参数类型  | 是否必填 | 参数说明 |
| ---             | ----    | ----    | ----   |
| authorization          | String     | 是   | Bearer加空格加授权的token，例如 "Bearer 21795f65-d8db-4b1a-a27e-cbebc08fcb11" |

### 参数列表
| 参数名称         | 参数类型  | 是否必填 | 参数说明 |
| ---             | ----    | ----    | ----   |
| clientId          | String     | 是   | 第三方client id |
| sign          | String     | 是   | 第三方参数签名 |

### 签名算法
  参数名ASCII码从小到大排序，最后拼接上第三方的key得到一个字符串，然后对这个字符串md5，得到签名字段。示例代码如下。
```
{
    String parmas = "clientId=client&key=aeofijslkadfoiwejfa"；
    String sign = md5(params);
    
}
```

## 响应

**同步返回**

```javascript
{
    "code":1,
    "data":{
        "avatar":"https://static.tinfinite.com/candy/dync/2941922_1541064461852_0",
        "nickName":"大漠斜阳西风烈酒",
        "phoneNum":"8613717536713",
        "openId":"1fea115e7e39432a20e0b9be46700f72"
    }
}
{
    "code":0,
    "err":{
        "err_code":10076,
        "message":"签名错误"
    }
}
```
### 返回值
| 参数名称         | 返回值类型  | 说明 |
| ---            | ----     | ----   |
| code          | int     | 1为成功，0为失败
| avatar          | String     | 用户头像url|
| nickName          | String     | 用户昵称|
| phoneNum          | String     | 用户手机号，如果授权范围不符合，这个字段不会有|
| openId          | String     | 用户在第三方平台的open id|
| err_code          | int     | 错误码|
| message          | String     | 错误描述|



