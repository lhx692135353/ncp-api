**接口文档**

**后台出入人口查询接口**

接口地址：/manage/find-cp
请求方式：GET

请求字段：

| 字段名称 | 字段类型 | 是否必填 | 标识 |
| -------- | -------- | -------- | ---- |


返回数据：

| 字段名称  | 字段类型 | 标识                     |
| --------- | -------- | ------------------------ |
| errorCode | int      | 返回200为成功,其他为失败 |
| message   | string   | 请求返回消息             |
| CpID      | int      | 采集人id                 |
| CpName    | string   | 采集人name               |
| Phone     | string   | 电话                     |
| Password  | string   | 密码                     |

````
{
    "attachment": {
        "collectionPerson": {
            "CpID": 5,
            "CpName": "刘帅",
            "Phone": "18111111111",
            "Password": "123123",
            "CreateDate": "2020-02-12T10:21:29+08:00",
            "ModifyDate": "2020-02-12T10:21:29+08:00"
        },
        "collectionSite": {
            "csId": 7,
            "csName": "采集点4",
            "csURL": "https://vicshow-1251558020.cos.ap-beijing.myqcloud.com/qr7.png",
            "createDate": "2020-02-12T10:20:51+08:00",
            "modifyDate": "2020-02-12T10:20:51+08:00"
        }
    },
    "errorCode": 200,
    "message": "查询成功"
}
````