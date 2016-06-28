# Proxy

* `npm install proxy-agent --save`
* In code:
```JavaScript
var proxy = require('proxy-agent');

AWS.config.update({
  httpOptions: { agent: proxy('http://internal.proxy.com') }
});

var s3 = new AWS.S3();
s3.getObject({Bucket: 'bucket', Key: 'key'}, function (err, data) {
  console.log(err, data);
});
```
