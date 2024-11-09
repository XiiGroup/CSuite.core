# Unified Xperience 360
Powerful API Library for interacting with UXP

# Sample PHP Usage
This sample php code creates a new contact into csuite for the platform whatsapp.
Replace **UXP_DOMAIN** , **API_USERNAME** & **API_KEY** with your csuite API Information, make sure you installed whatsapp plugin on UXP before using whatsapp platform.

```<?php
require_once('PHPUXP.php');
$uxp = new UXP("UXP_DOMAIN", "API_USERNAME", "API_KEY");
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
$uxp->payload($payload);
$response = $uxp->execute();
print_r($response);
```

For all api payloads key and values [Check wiki](https://github.com/xiigroup/UXPerience/wiki)
