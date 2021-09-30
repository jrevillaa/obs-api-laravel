# Huawei Cloud OBS for Laravel

[Huawei Cloud OBS](https://support.huaweicloud.com/devg-obs_php_sdk_doc_zh/zh-cn_topic_0132036136.html) 

# Requirement

- PHP >= 7.1.3

# Installation

```shell
$ composer require "jrevillaa/obs-api-laravel"
```

# Configuration

1. After installing the library, register the file:

  ```php
  // Import the class namespaces first, before using it directly
    use Obs\ObsClient as ObsClient;
    use Obs\ObsException as ObsException;
    
    $ak = '*** Provide your Access Key ***';
    
    $sk = '*** Provide your Secret Key ***';
    
    $endpoint = 'https://your-endpoint:443';
    
    $obsClient = ObsClient::factory(array (
        'key' => $ak,
        'secret' => $sk,
        'endpoint' => $endpoint,
    ));
  ```


# License

MIT
