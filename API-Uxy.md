# Index

* [1.1 Uxy Load](##-1.1-Uxy-Load)
* [1.2 Uxy Batch Load](##-1.2-Uxy-Batch-Load)
* [2.1 Uxy Update](##-2.1-Uxy-Update)
* [2.2 Uxy Batch Get](##-2.2-Uxy-Batch-Get)

# Content

## 1.1 Uxy Load

URL: /uxy/load  

RequestBody:  
```json
{
    "uxId": "uxid",
    "uyId": "uyid"
}
```

ResponseBody:  
```json
{
    "uxyId": "uxidVuyid",
    "uxId": "uxid",
    "uyId": "uyid",
    "applyFriend": true,
    "applyFriendTime": 1601234567890,
    "beFriend": true,
    "beFriendTime": 1601234567890,
    "remarkName": "jiefei",
    "showName": "jf"
}
```

Request Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|  uxyId  |  String  |  uxyId   |

Response Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|  uxyId  |  String  |  uxyId   |
|  uxId  |  String  |  uxId   |
|  uyId  |  String  |  uyId   |
|  applyFriend  |  Boolean  |  申请好友   |
|  applyFriendTime  |  Long  |  申请好友时间   |
|  beFriend  |  Boolean  |  成为好友   |
|  beFriendTime  |  Long  |  成为好友时间   |
|  remarkName  |  String  |  备注名   |
|  showName  |  String  |  显示名   |

## 1.2 Uxy Batch Load

URL: /uxy/batchLoad  

RequestBody:  
```json
{
    "uxyIds": [
        {
            "uxId": "uuid",
            "uyId": "uuid"
        }
    ]
}
```

ResponseBody:  
```json
[]
```

Request Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|  uxyIds  |  List(Uxy)  |  uxyId列表   |

Response Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|    |    |     |

## 2.1 Uxy Save

URL: /uxy/save  

RequestBody:  
```json
{
    "uyId": "asdf", 
    "applyFriend": true,
    "beFriend": true,
    "remarkName": "asdf",
    "showName": "asdf"
}
```

ResponseBody:  
```json
{}
```

Request Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|  uxyId  |  String  |  uxyId   |
|  applyFriend  |  Boolean  |  申请好友   |
|  beFriend  |  Boolean  |  成为好友   |
|  remarkName  |  String  |  备注名   |
|  showName  |  String  |  显示名   |

Response Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|    |    |     |

## 2.2 Uxy Batch Get

URL: /uxy/batchGet  

RequestBody:  
```json
{
    "asUx": true,
    "asUy": true, 
    "applyFriend": true,
    "beFriend": true
}
```

ResponseBody:  
```json
[]
```

Request Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|  asUx  |  Boolean  |  作为Ux   |
|  asUy  |  Boolean  |  作为Uy   |
|  applyFriend  |  Boolean  |  申请好友   |
|  beFriend  |  Boolean  |  成为好友   |

Response Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|    |    |     |
