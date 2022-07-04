# X-APPLICATION-VERSION

Example X-APPLICATION-VERSION simulate the required Header

```sh
curl  --resolve app.example.com:80:127.0.0.1 http://app.example.com

curl  --resolve app.example.com:80:127.0.0.1 http://app.example.com/1
curl  --resolve app.example.com:80:127.0.0.1 http://app.example.com/2
```

```sh
curl -v -iL --resolve app.example.com:80:127.0.0.1 http://app.example.com/1

curl -v -iL -H "X-APPLICATION-VERSION: 2048"  --resolve app.example.com:80:127.0.0.1 http://app.example.com/1

```
