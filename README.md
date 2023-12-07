# CSuite.core
Powerful API Library for interacting with CSuite

# Usage

```<?php
require_once('PHPCSuite.php');
$csuite = new CSuite("CSUITE_DOMAIN", "API_USERNAME", "API_KEY"); //CSUITE_DOMAIN - without leading http:// or https://, e.g. **yourdomain.com**
$payload = [
'create'=>true,
'platform'=>'whatsapp',
'firstname'=>'John',
'lastname'=>'Staayn',
'email'=>'j.staayn@biz.com',
'number'=>'270000000',
'notes'=>'',
];
$csuite->payload($payload);
$csuite_response = $csuite->execute();
print_r($csuite_response);
```
