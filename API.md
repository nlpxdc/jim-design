# Index

* [1.1 User Register By Username](##-1.1-User-Register-By-Username)
* [1.2 User Login By Username](##-1.2-User-Login-By-Username)

# Content

## 1.1 User Register By Username

URL: /user/registerByUsername  

RequestBody:  
```json
{
    "username": "cjf001",
    "nickname": "杰飞",
    "password": "123456",
}
```

ResponseBody:  
```json
{
    "userId": "UsUUID",
    "tokenIssueTime": 1590413448979,
    "accessToken": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiIxMTI5NjIyODQzIiwiaG90ZmFjZUlkIjozMzU5ODQ2NTU3NjI3ODg0NzM0LCJjbGllbnRTaWduYXR1cmUiOiJjYWJiMDJlYTFiZGI2ZGYwODI4NDY1MzJkZGY0ZTJjOWUwNmZlODViYmU4ZjRhODFmZGNmNDkyM2E4YzdhNzMwIiwiaXNzIjoid2F3YSIsInVzZXJUeXBlIjowLCJ0eXBlIjoiQWNjZXNzIiwiZXhwIjoxNTkwNDk5ODQ4LCJpYXQiOjE1OTA0MTM0NDgsInVzZXJJZCI6MTEyOTYyMjg0M30.95siySWk7lWvYnM8ubl9GrXTlwxht0QyQo6bV9WWWn4",
    "accessExpireTime": 1590499848979
}
```

Request Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|  username  | String   | 用户名    |
|  nickname  | String   | 昵称    |
|  password  | String   | 密码    |

Response Field  

| 字段     |     类型 |   描述   | 
| :--------------: | :--------:| :------: |
|  userId  | Long   | 用户Id    |
|  tokenIssueTime  | Long   | token签发时间    |
|  accessToken  | String   | Access Token    |
|  accessExpireTime  | Long   | Access Token 过期时间    |

## 1.2 User Login By Username

URL: /user/loginByUsername  

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
    "userId": 1129622843,
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
