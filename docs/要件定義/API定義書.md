# IDリポジトリAPI定義書

## リクエスト
```
GET http://localhost:4000/id/Users?filter=userName eq "[ログインID]"&attributes=externalId HTTP/1.1
Accept: application/scim+json
```

## レスポンス
```
HTTP/1.1 200 OK
Content-Type: application/scim+json;charset=UTF-8
Location: http://localhost:4000/id
{
  "schemas":["urn:ietf:param:scim:api:messages:2.0:ListResponse"],
  "totalResults":1,
  "Resources":[
    "id":"xxxxxxxxxx-xxxxxxxxxx",
    "externalId":"yyyyyyyyyy"
  ]
}
```
