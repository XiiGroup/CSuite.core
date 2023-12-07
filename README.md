# CSuite.core
Powerful API Library for interacting with CSuite

# Usage

```<?php
require_once('PHPCSuite.php');
$csuite = new CSuite("API_USERNAME", "API_KEY");

$payload = [
''=>,
''=>
];

$csuite->payload($payload);
$csuite_response = $csuite->execute();
```
