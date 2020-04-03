### 金山云点播转码 SDK

#### 使用方式

```javascript
const Client = require('ksc-kvs-sdk').Client;
const client = new Client({
    accessKeyId: '<accesskey id>',
    secretAccessKey: '<accesskey secret>',
    apiVersion: '2017-01-01',
});

client.request('<金山云接口名称>', userParams: {
        // 金山与接口所需参数, 其中 Action 与 Version 可以忽略
    },
    options: {
        headers?,
        timeout?,
        ...
    },
);
```

#### client.request 示例
查询 [模板列表接口](https://docs.ksyun.com/documents/2392)

```javascript
client.request('GetPresetList')
```
