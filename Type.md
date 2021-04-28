# Media
```json
{
    "mediaType": 1,
    "text": "asdf",
    "thumbUrl": "http://xxx.jpg",
    "originUrl": "http://xxx.jpg",
    "width": 720,
    "height": 1280,
    "duration": 4000
}
```

| 字段  | 类型  | 约束  |  说明 |
|---|---|---|---|
| mediaType  | Integer  | 非空  | 媒体类型（0保留，1文本、2图片、3音频、4视频）  |
| text  | String  |   | 文本  |
| thumbUrl  | String  |   | 缩略图Url  |
| originUrl  | String  |   | 原文件Url  |
| width  | Integer  |   | 宽度  |
| height  | Integer  |   | 高度  |
| duration  | Long  |   | 时长（毫秒）  |