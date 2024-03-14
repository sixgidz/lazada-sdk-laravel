# **Lazada PHP SDK for Laravel**

This PHP SDK is available to download at https://open.lazada.com  
  
Support Laravel 7.x / 8.x / 9.x / 10.x / 11.x

## **Installation**

 Via Composer  
   
 `composer require sixgidz/lazada-sdk-php`  

   ## **How to use**  
```php  
use Lazada\LazopClient;  
use Lazada\LazopRequest;

$c = new LazopClient(url,appkey,appSecret);
$request = new LazopRequest('/auth/token/create');
$request->addApiParam('code','0_100132_2DL4DV3jcU1UOT7WGI1A4rY91');
$request->addApiParam('uuid','This field is currently invalid,  do not use this field please');
var_dump($c->execute($request));
```

 https://open.lazada.com/apps/doc/api
