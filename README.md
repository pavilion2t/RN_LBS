# RN_LBS
使用express框架   
https://www.npmjs.com/package/express   
  ```
   $ npm install -g express-generator@4   
      //  基于ejs创建项目 
   $ express -e service  
   $ cd service && npm install
      // run the app:
   $ DEBUG=service:* npm start
  ```     
  
服务--架构、数据库、ORM模型、安全认证     

```
npm install -g supervisor   
supervisor bin/www   
```    

返回JSon数据   
```
var express = require('express');
var router = express.Router();

router.get('/', function(req, res, next) {
  // res.render('index', { title: 'Express' });
  return res.send({
    status: 1,
    info: "return sth"
  })
});

module.exports = router;   
```   

返回页面  
```
var express = require('express');
var router = express.Router();

router.get('/', function(req, res, next) {
  res.render('index', { title: 'Express' });
});

module.exports = router;   
```



