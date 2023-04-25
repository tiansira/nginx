# nginx 文件结构

```
...              #全局块

events {         #events块
   ...
}

http      #http块
{
    ...   #http全局块
    server        #server块
    { 
        ...       #server全局块
        location [PATTERN]   #location块
        {
            ...
        }
        location [PATTERN] 
        {
            ...
        }
    }
    server
    {
      ...
    }
    ...     #http全局块
}
```


```
[root@dtian-demo nginx-1.24]# pwd
/SCRATCH/nginx-1.24
[root@dtian-demo nginx-1.24]# ll
total 0
drwxrwxrwx 2 nginx nginx   6 Apr 24 17:59 client_body_temp
drwxrwxrwx 2 nginx nginx 333 Apr 25 21:41 conf
drwxr-xr-x 2 nginx nginx  25 Apr 25 21:47 conf.d
drwxrwxrwx 2 nginx nginx   6 Apr 24 17:59 fastcgi_temp
drwxrwxrwx 5 nginx nginx  77 Apr 25 14:27 html
drwxrwxrwx 2 nginx nginx  58 Apr 25 10:47 logs
drwxrwxrwx 2 nginx nginx   6 Apr 24 17:59 proxy_temp
drwxrwxrwx 2 nginx nginx  36 Apr 25 11:09 sbin
drwxrwxrwx 2 nginx nginx   6 Apr 24 17:59 scgi_temp
drwxrwxrwx 2 nginx nginx   6 Apr 24 17:59 uwsgi_temp
```