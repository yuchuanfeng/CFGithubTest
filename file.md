
### 上传文件
|  url | ?module=file&c=File&action=upload | 
|------|:-----------------------------------------------------:|
|  数据请求方式 | POST | 

|参数名称|类型|说明|必选|
|-------|:---:|:--:|:--:|
|token|string|token|是|
|file|文件类型|文件|是|

返回数据

```json
{
    "filePath": "20170710/59633e5773efa1.38188873.docx",
    "fileId": 60249,
    "fileName": "123.docx",
    "code": 1,
    "status": "OK"
}
```

### 删除文件
|  url | ?module=file&c=File&action=delete | 
|------|:-----------------------------------------------------:|
|  数据请求方式 | POST | 

|参数名称|类型|说明|必选|
|-------|:---:|:--:|:--:|
|token|string|token|是|
|fileId|int|文件ID|是|

返回数据

```json
{
    "code": 0,
    "status": "OK！"
}
```

### 文件列表
|  url | ?module=file&c=File&action=fetchAll | 
|------|:-----------------------------------------------------:|
|  数据请求方式 | POST | 

|参数名称|类型|说明|必选|
|-------|:---:|:--:|:--:|
|token|string|token|是|

返回数据

```json
{
    "code": 0,
    "status": "OK！",
    "list": [
        {
            "fileId": "91213",
            "userId": "10086",
            "addTime": "2017-07-07 19:21:19",
            "limitRead": "0",
            "limitWrite": "0",
            "limitDownload": "0",
            "fileName": "123.docx"
        },
        {
            "fileId": "92084",
            "userId": "8790",
            "addTime": "2017-07-07 14:53:51",
            "limitRead": "0",
            "limitWrite": "0",
            "limitDownload": "0",
            "fileName": "123.docx"
        },
        {
            "fileId": "92085",
            "userId": "1277",
            "addTime": "2017-07-07 19:52:46",
            "limitRead": "0",
            "limitWrite": "0",
            "limitDownload": "0",
            "fileName": "123.docx"
        }
    ]
}
```

### 修改文件内容
|  url | ?module=file&c=File&action=update | 
|------|:-----------------------------------------------------:|
|  数据请求方式 | POST | 

|参数名称|类型|说明|必选|
|-------|:---:|:--:|:--:|
|token|string|token|是|
|fileId|int|文件ID|是|
|file|文件类型|文件|是|

返回数据

```json
{
    "code": 0,
    "status": "OK！"
}
```
