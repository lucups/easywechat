# [EasyWeChat](https://easywechat.com)

## 环境需求

- PHP >= 8.0.2
- [Composer](https://getcomposer.org/) >= 2.0

## 安装

```bash
composer require lucups/easywechat:6.*
```

## 使用示例

基本使用（以公众号服务端为例）:

```php
<?php

use EasyWeChat\OfficialAccount\Application;

$config = [
    'app_id' => 'wx3cf0f39249eb0exxx',
    'secret' => 'f1c242f4f28f735d4687abb469072xxx',
    'aes_key' => 'abcdefghijklmnopqrstuvwxyz0123456789ABCDEFG',
    'token' => 'easywechat',
];

$app = new Application($config);

$app->getServer()->with(fn() => "您好！EasyWeChat！");

$response = $server->serve();
```

## 文档和链接

[官网](https://easywechat.com) · [讨论](https://github.com/w7corp/easywechat/discussions) · [更新策略](https://github.com/w7corp/easywechat/security/policy)

## License

MIT
