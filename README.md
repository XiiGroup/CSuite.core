# CSuite.core
Powerful API Library for interacting with CSuite

# Sample Usage
This sample php code creates a new contact into csuite for the platform whatsapp.
Replace **CSUITE_DOMAIN** , **API_USERNAME** & **API_KEY** with your csuite API Information

```<?php
require_once('PHPCSuite.php');
$csuite = new CSuite("CSUITE_DOMAIN", "API_USERNAME", "API_KEY"); //CSUITE_DOMAIN - without leading http:// or https://, e.g. **yourdomain.com**
$payload = [
'endpoint'=>'contacts',
'action'=>'new',
'platform'=>'whatsapp',
'firstname'=>'Sipho',
'lastname'=>'Selabe',
'email'=>sipho@email.com,
'number'=>'00000000',
'notes'=>'Client lead'
];
$csuite->payload($payload);
$csuite_response = $csuite->execute();
print_r($csuite_response);
```

For all api payloads key and values [Check wiki](https://github.com/xiigroup/CSuite.core/wiki)
