# phalcon-docker-nginx

```
$ phalcon project --name=Demo --enable-webtools --type=simple                                                                                                                                                        ✔  10565  01:16:28 

Phalcon DevTools (3.4.0)


  Success: Controller "index" was successfully created.

/Users/****/Demo/app/controllers/IndexController.php

  Success: Project 'Demo' was successfully created.
Please choose a password and username to use Database connection.Used default:'root' without password.
```

![image](https://user-images.githubusercontent.com/400362/51873248-1905f280-2365-11e9-9937-247b673d1522.png)

*access.log*
```
192.168.112.1 - - [28/Jan/2019:23:18:59 +0000] "GET / HTTP/1.1" 502 559 "-" "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_13_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/71.0.3578.98 Safari/537.36"
```

*error.log*
```
2019/01/28 23:18:59 [error] 6#6: *2 recv() failed (104: Connection reset by peer) while reading response header from upstream, client: 192.168.112.1, server: , request: "GET / HTTP/1.1", upstream: "fastcgi://192.168.112.2:9000", host: "localhost:8080"
```

**PHP 7.2.14**
![image](https://user-images.githubusercontent.com/400362/51873511-21aaf880-2366-11e9-89f4-990738c255c1.png)
