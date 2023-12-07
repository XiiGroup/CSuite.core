# CSuite.core
Powerful API Library for interacting with CSuite

# Sample PHP Usage
This sample php code creates a new contact into csuite for the platform whatsapp.
Replace **CSUITE_DOMAIN** , **API_USERNAME** & **API_KEY** with your csuite API Information, make sure you installed whatsapp plugin on csuite before using whatsapp platform.

```<?php
require_once('PHPCSuite.php');
$csuite = new CSuite("CSUITE_DOMAIN", "API_USERNAME", "API_KEY");
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
