#腾讯云对象存储V4
官方提供的版本并不支持composer, 官方回复支持也已经是1年之前的事情了....

目测等待官方版本已经是毫无希望了.


目前主要实现了对象化调用. 具体代码如下:


`<?php

use qcloudcos\Cosapi;


$api = new Cosapi($appID, $secretID, $secretKey, $bucket);

//上传文件
$api->FileUpload($file,$key);
//删除文件
$api->FileDelete($key);

`