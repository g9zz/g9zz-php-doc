# g9zz-php-doc

## 后台

### post

* [帖子列表](#帖子列表)

## 前台



## 后台

### post

#### 帖子列表

- PATH `console/post`
- METHOD `GET`
- PARAMS

| request        | param    |  note  | other |
| --------   | -----:   | :----: | ---- |
|replyCount|`desc`,`asc`| 回复数 | |
|viewCount|`desc`,`asc`|点击数||
|voteCount|`desc`,`asc`|点赞数|
|isTop|`desc`,`asc`|置顶|
|isExcellent|`desc`,`asc`|精华|
|isBlocked|`desc`,`asc`|折叠|
|isTagged|`desc`,`asc`|被标签|

- RESPONSE

```json
{
  "code": 0,
  "message": "成功",
  "data": [
    {
      "id": 1,
      "title": "这是标题",
      "content": "这个是内容",
      "source": "IOS",
      "replyCount": 0,
      "viewCount": 100,
      "voteCount": 1,
      "order": 0,
      "isTop": "yes",
      "isExcellent": "yes",
      "isBlocked": "no",
      "bodyOriginal": null,
      "excerpt": null,
      "isTagged": "no",
      "user": {
        "name": "叶落",
        "avatar": "https://image.baidu.com/search/detail?ct=503316480&z=undefined&tn=baiduimagedetail&ipn=d&word=宠物&step_word=&ie=utf-8&in=&cl=2&lm=-1&st=undefined&cs=3495161387,2602242859&os=3408035920,2765980592&simid=4249158544,682669875&pn=1&rn=1&di=170437508230&ln=1986"
      },
      "lastReplyUser": {
        "name": "叶落",
        "avatar": "https://image.baidu.com/search/detail?ct=503316480&z=undefined&tn=baiduimagedetail&ipn=d&word=宠物&step_word=&ie=utf-8&in=&cl=2&lm=-1&st=undefined&cs=3495161387,2602242859&os=3408035920,2765980592&simid=4249158544,682669875&pn=1&rn=1&di=170437508230&ln=1986"
      }
    }
  ],
  "pager": {
    "entities": 1,
    "current": 1,
    "total": 1,
    "limit": 20,
    "last": 1,
    "next": "",
    "previous": ""
  }
}
```

