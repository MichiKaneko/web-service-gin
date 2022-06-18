# web-service-gin
## 使い方
```
go run .
```

## リクエスト
全アルバムを取得
http://localhost:8080/albums

IDを指定してアルバムを取得
http://localhost:8080/albums/{ID}

アルバムを追加（POSTなので、コンソールから追加）
```
 curl http://localhost:8080/albums \
    --include \
    --header "Content-Type: application/json" \
    --request "POST" \
    --data '{"id": "4","title": "The Modern Sound of Betty Carter","artist": "Betty Carter","price": 49.99}'
```
