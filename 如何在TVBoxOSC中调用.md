## 参数说明
|参数|是否必填|默认值|功能|
| :----: | :----: | :----: | :----: |
|`sites`|否|`all`|可筛选站点，多个站点用,隔开|
|`ali_token`|否|`无`|提供阿里系的搜索播放功能（非必须）|
|`timeout`|否|`5`|提供服务端搜索限时返回结果功能，超时数据不再等待|
## json示例（请修改为自己的`IP:PORT`或域名，注意默认调用路径`/vod`）
```
{
    "sites":[
        {
            "key":"t4test",
            "name":"T4测试",
            "type":4,
            "api":"http://[ip]:[port]/vod?sites=all&ali_token=3xx9cfxxxx509bxx&timeout=5",
            "searchable":1,
            "quickSearch":1,
            "filterable":0
        }
    ]
}
```