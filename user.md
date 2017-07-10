### 登录 
|  url | http://www.jiami.com?module=user&c=User&action=login | 
|------|:-----------------------------------------------------:|
|  数据请求方式 | POST | 

|参数名称|类型|说明|必选|
|-------|:---:|:--:|:--:|
|userName|string|用户名|是|
|pwd|string|密码|是|

返回数据

```json
{
    "code": 1,
    "status": "OK",
    "userInfo": {
        "userId": "10086",
        "userName": "admin",
        "registerTime": "2017-10-12",
        "isAdmin": "1",
        "limitLevel": "9",
        "token": "79f7bc501354569cdf58042d357ef3e5"
    }
}
```

### 管理员添加普通用户
|  url | ?module=user&c=User&action=addUser | 
|------|:-----------------------------------------------------:|
|  数据请求方式 | POST | 

|参数名称|类型|说明|必选|
|-------|:---:|:--:|:--:|
|userName|string|用户名|是|
|pwd|string|密码|是|
|token|string|token|是|
|level|int|权限值|否|

返回数据

```json
{
    "code": 1,
    "status": "OK",
    "userInfo": {
        "userId": "5660",
        "userName": "liu1",
        "registerTime": "2017-07-10 16:26:39",
        "isAdmin": "0",
        "limitLevel": "0"
    }
}
```

### 管理员移除普通用户
|  url | ?module=user&c=User&action=removeUser | 
|------|:-----------------------------------------------------:|
|  数据请求方式 | POST | 

|参数名称|类型|说明|必选|
|-------|:---:|:--:|:--:|
|userId|int|用户ID|是|
|token|string|token|是|

返回数据

```json
{
    "code": 1,
    "status": "OK"
}
```
### 登出
|  url | ?module=user&c=User&action=logout | 
|------|:-----------------------------------------------------:|
|  数据请求方式 | POST | 

|参数名称|类型|说明|必选|
|-------|:---:|:--:|:--:|
|token|string|token|是|

返回数据

```json
{
    "code": 1,
    "status": "OK"
}
```
