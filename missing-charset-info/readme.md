Missing character information, better known as `ERR_MISSING_CHARSET` doesn't exist!

![error-doesn't-exist](../screenshots/2025-04-03-20-18-42.png)

I tried reproduce the issue using:

```bash
➜ echo -ne "HTTP/1.1 200 OK\r\n\r\n<html><body>Hello</body></html>" | nc -l -p 8080
```

Which actually returned hello normally.

![hello](../screenshots/2025-04-03-20-23-18.png)
