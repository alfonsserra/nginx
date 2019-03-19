# nginx

To install and launch Nginx, use the command:

```
brew install nginx
```

Docroot is set to /usr/local/var/www, and nginx will load all files in /usr/local/etc/nginx/servers/.

To have launchd start nginx now and restart at login:

```
brew services start nginx
```
The default port is set in /usr/local/etc/nginx/nginx.conf. If you set the port to 80, must run with sudo:

```
sudo brew services start nginx
```

If you don't want/need a background service you can just run:

```
nginx
```

Use:

```
nginx -s signal     
```

to send signal to a master process: stop, quit, reopen, reload
