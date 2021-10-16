# How to use this patch

## PHPMailer

Deploy PHPMailer classes in a directory named `phpmailer` located in the root directory of your instance.

## Patch

```bash
cd <YOUR JIRAFEAU INSTANCE PATH>
wget https://raw.githubusercontent.com/betaglop/jirafeau-email-alert-patch/main/jirafeau.patch -O - | patch -p0
```

## Setup

Do not forget seting the parameter `contactperson` in your `lib/config.local.php`.

## Test

Test your configuration and... it's done.

Do not forget checking your spambox... in case the email is considered as a spam.
