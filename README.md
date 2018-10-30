# 腾讯云对象存储 COS 使用实例

> 来源自腾讯云的 [JavaScript SDK 仓库](https://github.com/tencentyun/cos-js-sdk-v5) 和 [Node.js SDK 仓库](https://github.com/tencentyun/cos-nodejs-sdk-v5)，并在其基础上稍作调整。

`index.html` ——> https://github.com/tencentyun/cos-js-sdk-v5/blob/master/demo/sts-put.html

`server/sts-auth.js` ——> https://github.com/tencentyun/cos-js-sdk-v5/blob/master/server/sts-auth.js

`server/sts-auth.php` ——> https://github.com/tencentyun/cos-js-sdk-v5/blob/master/server/sts-auth.php

`utils/getAuth.js` ——> https://github.com/tencentyun/cos-nodejs-sdk-v5/blob/master/sdk/util.js

你需要一定的前置条件才能跑通本 Demo， 具体参考：[腾讯云文档](https://cloud.tencent.com/document/product/436/9067)。诸如 `SecretId` 和 `SecretKey` 等敏感信息已替换为 ****** 脱敏，你需要替换成自己的。使用我的个人账号，本 Demo 亲测可用。

## 启动计算签名服务（二选一）

#### 1.启动 Node 服务

根目录下执行 `node ./server/sts-auth.js`

#### 2.启动 PHP 服务

`server/sts-auth.php` 文件需运行在本地 `8888` 端口