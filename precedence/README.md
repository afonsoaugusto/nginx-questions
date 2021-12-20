# Test-AB

Example test-AB simulate the Optimize function

```sh
curl  --resolve app.example.com:80:127.0.0.1 http://app.example.com

curl  --resolve app.example.com:80:127.0.0.1 http://app.example.com/1
curl  --resolve app.example.com:80:127.0.0.1 http://app.example.com/2

curl  --resolve app_a.example.com:80:127.0.0.1 http://app_a.example.com

curl  --resolve app_b.example.com:80:127.0.0.1 http://app_b.example.com
```

```sh
curl -v -iL --resolve app.example.com:80:127.0.0.1 http://app.example.com?v=1

curl -v -iL --cookie "site_version=app_a_up" --resolve app.example.com:80:127.0.0.1 http://app.example.com

```
