# Index

* [1.1.1 Uxy Load As Ux By Uy](##-1.1.1-Uxy-Load-As-Ux-By-Uy)
* [1.1.2 Uxy Load As Uy By Ux](##-1.1.2-Uxy-Load-As-Uy-By-Ux)
* [2.1 Uxy Apply Friend](##-2.1-Uxy-Apply-Friend)
* [2.2 Uxy Batch Get New Friend](##-2.2-Uxy-Batch-Get-New-Friend)

# Content

## 1.1.1 Uxy Load As Ux By Uy

URL: /uxy/loadAsUxByUy  

RequestBody:  
```json
{
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
|  uyId  |  String  |  uyId   |

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

## 1.1.2 Uxy Load As Uy By Ux

URL: /uxy/loadAsUyByUx  

RequestBody:  
```json
{
    "uxId": "uxid"
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
|  uxId  |  String  |  uxId   |

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


## 2.1 Uxy Apply Friend

URL: /uxy/applyFriend  

RequestBody:  
```json
{
    "uyId": "uyid"
}
```

ResponseBody:  
```json
{}
```

Request Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|  uyId  |  String  |  uyId   |

Response Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|    |    |     |

## 2.2 Uxy Batch Get New Friend

URL: /uxy/batchGetNewFriend  

ResponseBody:  
```json
[]
```

Response Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|    |    |     |

## 2.3 Uxy Agree Friend

URL: /uxy/agreeFriend  

RequestBody:  
```json
{
    "userId": "uuid"
}
```

Request Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|  uxId  |  String  |  uxId   |
