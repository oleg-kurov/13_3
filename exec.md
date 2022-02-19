**for db**
root@cp1:/home/rattle# kubectl exec postgres-0 -- ls -la  
total 72  
drwxr-xr-x    1 root     root          4096 Feb 12 16:14 .  
drwxr-xr-x    1 root     root          4096 Feb 12 16:14 ..  
drwxr-xr-x    1 root     root          4096 Feb 12 00:43 bin  
drwxr-xr-x    5 root     root           360 Feb 12 16:14 dev  
drwxr-xr-x    2 root     root          4096 Nov 30 04:59 docker-entrypoint-initdb.d  
drwxr-xr-x    1 root     root          4096 Feb 12 16:14 etc  
drwxr-xr-x    2 root     root          4096 Nov 24 09:20 home  
drwxr-xr-x    1 root     root          4096 Feb 12 00:43 lib  
drwxr-xr-x    5 root     root          4096 Nov 24 09:20 media  
drwxr-xr-x    2 root     root          4096 Nov 24 09:20 mnt  
drwxr-xr-x    2 root     root          4096 Nov 24 09:20 opt  
dr-xr-xr-x  269 root     root             0 Feb 12 16:14 proc  
drwx------    1 root     root          4096 Feb 18 10:31 root  
drwxr-xr-x    1 root     root          4096 Feb 12 16:14 run  
drwxr-xr-x    1 root     root          4096 Feb 12 00:43 sbin  
drwxr-xr-x    2 root     root          4096 Nov 24 09:20 srv  
dr-xr-xr-x   13 root     root             0 Feb 12 16:14 sys  
drwxrwxrwt    1 root     root          4096 Feb 12 00:43 tmp  
drwxr-xr-x    1 root     root          4096 Feb 12 00:43 usr  
drwxr-xr-x    1 root     root          4096 Feb 12 00:43 var  


**for back**  
root@cp1:/home/rattle# kubectl exec back-cfbb5c4cf-pfpkb -- ls -la  
total 28  
drwxr-xr-x 1 root root  4096 Feb 12 15:21 .  
drwxr-xr-x 1 root root  4096 Feb 18 10:49 ..  
-rw-rw-r-- 1 root root   280 Feb 12 14:57 Pipfile  
-rw-rw-r-- 1 root root 11276 Feb 12 14:57 Pipfile.lock  
-rw-rw-r-- 1 root root  2291 Feb 12 14:57 main.py  

**for front**  
root@cp1:/home/rattle# kubectl exec front-784597b7cd-gjwh2 -- ls -la  
total 420  
drwxr-xr-x 1 root root   4096 Feb 12 15:31 .  
drwxr-xr-x 1 root root   4096 Feb 18 10:54 ..  
-rw-rw-r-- 1 root root     30 Feb 12 14:57 .env  
-rw-rw-r-- 1 root root     30 Feb 12 14:57 .env.example  
-rw-rw-r-- 1 root root    387 Feb 12 14:57 Dockerfile  
drwxrwxr-x 2 root root   4096 Feb 12 14:57 build  
-rw-rw-r-- 1 root root    344 Feb 12 14:57 demo.conf  
-rw-rw-r-- 1 root root    448 Feb 12 14:57 index.html  
-rw-rw-r-- 1 root root    344 Feb 12 14:57 item.html  
drwxrwxr-x 2 root root   4096 Feb 12 14:57 js  
-rw-rw-r-- 1 root root     80 Feb 12 14:57 list.json  
-rw-rw-r-- 1 root root 364679 Feb 12 14:57 package-lock.json  
-rw-rw-r-- 1 root root   1107 Feb 12 14:57 package.json  
drwxrwxr-x 2 root root   4096 Feb 12 14:57 static  
drwxrwxr-x 3 root root   4096 Feb 12 14:57 styles  
-rw-rw-r-- 1 root root   2781 Feb 12 14:57 webpack.config.js  
