Ta的主页-配音
===

| 提交格式        | 状态   |  版本  | 添加人 | 添加时间 | 修改人 | 修改时间 | 修改内容
| --------   | -----  | ----  |
| POST-JSON     | 待审核 |   v1.0    | 王学兴 | 2017-05-10 | | | | 
| POST-JSON     | 待审核 |   v2.0    | 王学兴 | 2017-05-10 | 王学兴| 2017-06-05| 修改language为transLang|

|URL|
|--|
|http://10.5.110.215:8088/IOL_ME5/userCenter/userHomePageDubb/|

请求参数
`````
{
   taUserId:"1234",//用户ID
   pageNum:1,//页码
   pageSize:20 //每页显示几条
}
```
返回结果（成功）
```
{
result：1,
data:{
  userId: 1234, //译员ID
  nickName:"成吉思汗", //昵称
  headPhoto:"http://7xl9b8.dl1.z0.glb.clouddn.com/242443424", //头像路径
  followCount: 200, //关注人数
  fansCount:130, //粉丝人数
  isFollow:0, //登录用户是否已关注此用户，0未关注；>0表示已关注
  dubbing:[
	{
	   videoId: 1234,//素材视频ID
	   name: "特大好消息",//视频名称
	   picPath:"http://7xl9b8.dl1.z0.glb.clouddn.com/242443424",//封面图片七牛路径
	   source:"动物世界",//视频来源
	   duration:120,//视频时长（s）
	   dubbingId:1234 //配音ID
	   transLang:"英语" //字幕语种
	},
	{
	   videoId: 1234,//素材视频ID
	   name: "特大好消息",//视频名称
	   picPath:"http://7xl9b8.dl1.z0.glb.clouddn.com/242443424",//封面图片七牛路径
	   source:"动物世界",//视频来源
	   duration:120,//视频时长（s）
	   dubbingId:1234 //配音ID
	   transLang:"英语" //字幕语种
	}
  ]
}
```
返回结果（失败）
```
{
result：0,
code:2001,
msg:"没找到对应数据"
}
```

