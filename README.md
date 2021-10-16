# How to use this patch

## PHPMailer

Deploy PHPMailer classes in a directory named `phpmailer` located in the root directory of your instance.

## Patch

```bash
cd <YOUR JIRAFEAU INSTANCE PATH>
wget https://raw.githubusercontent.com/betaglop/jirafeau-email-alert-patch/main/jirafeau.patch -O - | patch -p0
```

## Setup

Do not forget setting the following parameters in your `lib/config.local.php` file:

* `$cfg['contactperson'] = 'contact@yourdomain.tld'` and
* `$cfg['smtp'] = array('host' => 'smtp.yourdomain.tld', 'port' => 25),`

## Test

Test your configuration and... it's done.

Do not forget checking your spambox... in case the email is considered as a spam.
