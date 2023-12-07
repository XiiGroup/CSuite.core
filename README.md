# CSuite.core
Powerful API Library for interacting with CSuite

# Usage

```<?php
require_once('PHPCSuite.php');
$csuite = new CSuite("CSUITE_DOMAIN", "API_USERNAME", "API_KEY"); //CSUITE_DOMAIN - without leading http:// or https://, e.g. **yourdomain.com**
$payload = []; //payload as key=>value array
$csuite->payload($payload);
$csuite_response = $csuite->execute();
print_r($csuite_response);
```

For all api payloads key and values [Check wiki](https://github.com/xiigroup/CSuite.core/wiki)
