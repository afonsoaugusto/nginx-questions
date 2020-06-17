# Authorization

Example authorization simulate the required Header

```sh
curl  --resolve app.example.com:80:127.0.0.1 http://app.example.com

curl  --resolve app.example.com:80:127.0.0.1 http://app.example.com/1
curl  --resolve app.example.com:80:127.0.0.1 http://app.example.com/2
```

```sh
curl -v -iL --resolve app.example.com:80:127.0.0.1 http://app.example.com/1

curl -v -iL -H "authorization: ww4vhuM6PSKxbXkjTdmkKcmRxWyMErGg43YHyZApvcPRhBeGWXemrABPvKpcMwE"  --resolve app.example.com:80:127.0.0.1 http://app.example.com/1

```
