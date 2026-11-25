# FyraInput-Keyboard-Mouse PHP SDK

<!-- simple-start:start -->
Use FyraInput-Keyboard-Mouse from a PHP app.

**Start here.** Run `composer require titancsa/fyrainput-keyboard-mouse`, then try the short example below. Install the matching Windows driver separately.
<!-- simple-start:end -->

> [!IMPORTANT]
> **Contact TitanCSA**
>
> On [Discord](https://discord.com/app), choose **Friends → Add Friend**, enter **`titancsa`** and send the project name. Ask about commercial licensing, integration or support for this project.

`composer require titancsa/fyrainput-keyboard-mouse`

PHP 8.2+ Windows x64, extension FFI and `ffi.enable=true` are required. Matching driver installed separately; licensing and trial rules remain unchanged. Supported families: keyboard, mouse.

```php
require "vendor/autoload.php";
$client = new \TitanCSA\Products\FyraInputKeyboardMouse\Interceptor();
try { print_r($client->info()); } finally { $client->close(); }
```

See [API](docs/API.md). Installation and construction do not start input capture.
