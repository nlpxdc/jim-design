# Index

## I
* [0.1 UserLogin Register By Username](##-0.1-UserLogin-Register-By-Username)
* [0.2 UserLogin Login By Username](##-0.2-UserLogin-Login-By-Username)

## II
* [1.1 UserBase Get Profile](##-1.1-UserBase-Get-Profile)
* [1.2 UserBase Update Profile](##-1.2-UserBase-Update-Profile)

# Content

## 0.1 UserLogin Register By Username

URL: /userLogin/registerByUsername  

RequestBody:  
```json
{
    "username": "cjf001",
    "password": "123456"
}
```

ResponseBody:  
```json
{
    "userId": "Uuuid",
    "tokenIssueTime": 1590413448979,
    "accessToken": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiIxMTI5NjIyODQzIiwiaG90ZmFjZUlkIjozMzU5ODQ2NTU3NjI3ODg0NzM0LCJjbGllbnRTaWduYXR1cmUiOiJjYWJiMDJlYTFiZGI2ZGYwODI4NDY1MzJkZGY0ZTJjOWUwNmZlODViYmU4ZjRhODFmZGNmNDkyM2E4YzdhNzMwIiwiaXNzIjoid2F3YSIsInVzZXJUeXBlIjowLCJ0eXBlIjoiQWNjZXNzIiwiZXhwIjoxNTkwNDk5ODQ4LCJpYXQiOjE1OTA0MTM0NDgsInVzZXJJZCI6MTEyOTYyMjg0M30.95siySWk7lWvYnM8ubl9GrXTlwxht0QyQo6bV9WWWn4",
    "accessExpireTime": 1590499848979
}
```

Request Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|  username  | String   | 用户名    |
|  password  | String   | 密码    |

Response Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|  userId  | Long   | 用户Id    |
|  tokenIssueTime  | Long   | token签发时间    |
|  accessToken  | String   | Access Token    |
|  accessExpireTime  | Long   | Access Token 过期时间    |

## 0.2 UserLogin Login By Username

URL: /userLogin/loginByUsername  

RequestBody:  
```json
{
    "username": "cjf001",
    "password": "123456"
}
```

ResponseBody:  
```json
{
    "userId": "Uuuid",
    "tokenIssueTime": 1590413448979,
    "accessToken": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiIxMTI5NjIyODQzIiwiaG90ZmFjZUlkIjozMzU5ODQ2NTU3NjI3ODg0NzM0LCJjbGllbnRTaWduYXR1cmUiOiJjYWJiMDJlYTFiZGI2ZGYwODI4NDY1MzJkZGY0ZTJjOWUwNmZlODViYmU4ZjRhODFmZGNmNDkyM2E4YzdhNzMwIiwiaXNzIjoid2F3YSIsInVzZXJUeXBlIjowLCJ0eXBlIjoiQWNjZXNzIiwiZXhwIjoxNTkwNDk5ODQ4LCJpYXQiOjE1OTA0MTM0NDgsInVzZXJJZCI6MTEyOTYyMjg0M30.95siySWk7lWvYnM8ubl9GrXTlwxht0QyQo6bV9WWWn4",
    "accessExpireTime": 1590499848979
}
```

Request Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
| username   | String   | 用户名    |
| password   | String   | 密码  |

Response Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|  userId  | Long   | 用户Id    |
|  tokenIssueTime  | Long   | token签发时间    |
|  accessToken  | String   | Access Token    |
|  accessExpireTime  | Long   | Access Token 过期时间    |

## 1.1 UserBase Get Profile

URL: /userBase/getProfile  

ResponseBody:  
```json
{
    "userId": "Uuuid",
    "username": "cjf001",
    "nickname": "杰飞",
    "avatar": "http://xxx.jpg",
    "birthday": 1601234567890,
    "gender": 2,
    "area": "上海"
}
```

Response Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|  userId  | String   | 用户Id    |
|  username  |  String  |  用户名   |
|  nickname  |  String  |  昵称   |
|  avatar  |  String  |  头像   |
|  birthday  |  Long  |  生日   |
|  gender  |  Integer  |  性别（0保密，1男，2女）   |
|  area  |  String  |  地区   |

## 1.2 UserBase Update Profile

URL: /userBase/updateProfile  

RequestBody:  
```json
{
    "nickname": "杰飞",
    "avatar": "http://xxx.jpg",
    "birthday": 1601234567890,
    "gender": 2,
    "area": "上海"
}
```

Request Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|  nickname  |  String  |  昵称   |
|  avatar  |  String  |  头像   |
|  birthday  |  Long  |  生日   |
|  gender  |  Integer  |  性别（0保密，1男，2女）   |
|  area  |  String  |  地区   |
