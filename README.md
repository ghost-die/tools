# ghost-tools

**RSA签名类**

    $publickey = 'MFwwDQYJKoZIhvcNAQEBBQADSwAwSAJBAKm2fXfToHXPZwRXZLOkOsBZj2xOsvxEJgGl7XnlpKVtqivxT/zKIecdEnOnZ81UhhhqpsxREhVI66bHHKOpAq8CAwEAAQ==';
    
    $privkey = 'MIIBUwIBADANBgkqhkiG9w0BAQEFAASCAT0wggE5AgEAAkEAqbZ9d9Ogdc9nBFdks6Q6wFmPbE6y/EQmAaXteeWkpW2qK/FP/Moh5x0Sc6dnzVSGGGqmzFESFUjrpscco6kCrwIDAQABAkAH0LmSbRJ0mmp6DrQ6eZOjC/zI1g70AwdlCAkZlfOxEnqGxeNRwnQrFp/tMjaFm1cEOPYXN5tk/J+Y92R4iOfxAiEA37xJ3ldqZ/o5L7ehaph3URX9a9LsopMRSy/1Ph6SiX0CIQDCL9S7eR1mU8y6NB9115GpFhuaTTl2afS8UkLnLZoUmwIgDvIrFRlN2GhUzaU8uTw6LEaFyWArwqiEbTtk7KNqMpkCIDlkvbFzSJc36WiXgzznK+wX1qyyamtvQaBvh8qgFcxFAiA93MHzqsYkH0WgPd9W7xp/C0ZLq8muNhyAfpripx1ufA==';
    
    $rsa = new Rsa($publickey,$privkey);
    
    $str = $rsa->privEncrypt('ghost');  //加密
    
    $rsa->pubDecrypt($str); //解密

**Form 表单元素生成**

    FormBuilder::instance()->selectMonth('month');


**Pinyin 中文转拼音**

    Pinyin::get('张三',FALSE,'',TRUE);
    
    
**Random 随机生成**
    
    Random::uuid();

**Http 字符串** 

    Http::post('https://www.baidu.com');
    