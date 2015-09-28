github-webhook-handler-php
=====

#### 1. Add a weebhook in the Settings/Webhooks page of your respostory.

#### 2. Update the `$secret` and `$path` in the  `github-webhook-handler.php`.

#### 3. Upload `github-webhook-handler.php` to your server and copy the URL to it.

#### 4. Fill in the webhooks page.

#### 5. ssh to your server.

```bash
#if you are using Apache as web server, change `www-data` to `www`
chown -R www-data /path/to/the/repository/
chmod -R g+s /path/to/the/repository/
cd /path/to/the/repository/
sudo -u www-data git pull
```

#### 6. Done.
