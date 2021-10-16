# How to install this patch

## PHPMailer

Install PHPMailer in your instance in a directory named `PHPMailer`

## Patch

```bash
cd <YOUR JIRAFEAU INSTANCE PATH>
wget https://raw.githubusercontent.com/betaglop/jirafeau-email-alert-patch/main/jirafeau.patch -O - | patch -p0
```

## Setup

Do not forget seting the parameter `contactperson` in your `lib/config.local.php`.

## Test

Test your configuration and... it's done.
