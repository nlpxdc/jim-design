# Message
| 字段  | 类型  | 约束  |  说明 |
|---|---|---|---|
| messageId  | String  | 主键  | 消息Id（MSGsUUID）  |
| conversationId  | String  | 非空，Hash索引  | 对话Id  |
| sendTime  | Long  | 非空，Sort索引  | 发送时间  |
| sendUserId  | String  | 非空  | 发送者用户Id  |
| contentType  | Integer  | 非空  | 内容类型（0保留，1文本、2图片、3音频、4视频）  |
| text  | String  |   | 文本  |
| mime  | String  |   | MIME  |
| thumbUrl  | String  |   | 缩略图Url  |
| originUrl  | String  |   | 原图Url  |
| width  | Integer  |   | 宽度  |
| height  | Integer  |   | 高度  |
| duration  | Long  |   | 时长  |

# Conversation
| 字段  | 类型  | 约束  |  说明 |
|---|---|---|---|
| conversationId  | String  | 主键  | 对话Id（CVSsUUID）  |
| type  | Integer  | 非空  | 类型（0保留，1单聊，2群聊）  |
| name  | String  |   | 上次消息Id  |
| createTime  | Long  | 非空  | 创建时间  |
| lastMessageId  | String  | 非空  | 最后一条消息Id  |
| holdUserId  | String  | 非空  | 持有者用户Id  |

# User
| 字段  | 类型  | 约束  |  说明 |
|---|---|---|---|
| userId  | String  | 主键  | 用户Id（UsUUID）  |
| username  | String  | 非空，唯一，Hash索引  | 用户名  |
| loginPassword  | String  | 非空  | 登录密码  |
| nickname  | String  | 非空  | 昵称  |
| avatar  | String  |   | 头像  |
| birthday  | Long  |   | 地区  |
| gender  | Integer  |   | 性别（0保密，1男，2女）  |
| area  | String  |   | 地区  |

# UserConversation
| 字段  | 类型  | 约束  |  说明 |
|---|---|---|---|
| userConversationId  | String  | 主键  | 用户对话Id（UCsUUID）  |
| userId  | String  | 非空，Hash索引  | 用户Id  |
| conversationId  | String  | 非空，Hash索引  | 对话Id  |
| joinTime  | Long  | 非空  | 加入时间  |
| muteEnabled  | Boolean  |   | 静音  |

# UxUy
| 字段  | 类型  | 约束  |  说明 |
|---|---|---|---|
| uxuyId  | String  | 主键  | uxuyId（UsXIDxUsYID）  |
| uxId  | String  | 非空，Hash索引  | uxId  |
| uyId  | String  | 非空，Hash索引  | uyId  |
| beFriend  | Boolean  |   | 朋友  |
| beFriendTime  | Long  |   | 成朋友时间  |
| remarkName  | String  |   | 备注名  |
| showName  | String  |   | 显示名  |
