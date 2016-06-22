github-webhook-handler-php
=====

- Add a weebhook in the Settings/Webhooks page of your respostory.

- Update the `$secret` and `$path` in the  `github-webhook-handler.php`.

- Upload `github-webhook-handler.php` to your server and copy the URL to it.

- Fill in the webhooks page.

- ssh to your server.

```bash
#if you are using Apache as web server, change `www-data` to `apache`
chown -R www-data /path/to/the/repository/
chmod -R g+s /path/to/the/repository/
cd /path/to/the/repository/
sudo -u www-data git pull
```

- Save your webhook.

- Reference:
>- http://www.lovelucy.info/auto-deploy-website-by-webhooks-of-github-and-gitlab.html
>- http://www.v2ex.com/t/224238#2


- Repository deploy key setting.
```bash
    run ssh-keygen...
    add public key in deploy keys
    ssh-add to add the private key
    test with cmd: ssh -T git@github.com
    change the repository .git/config url to git@github.com:who/reposotiry.git
    run cmd git pull to test.
```

>- https://developer.github.com/guides/managing-deploy-keys/
>- https://segmentfault.com/a/1190000002645623




