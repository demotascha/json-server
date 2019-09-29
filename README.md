# json-server
Fake API server based on https://github.com/typicode/json-server

### Prepare your data

Create/Update a `db.json` file with some data
```
{
  "posts": [
    { "id": 1, "title": "json-server", "author": "typicode" }
  ],
  "comments": [
    { "id": 1, "body": "some comment", "postId": 1 }
  ],
  "profile": { "name": "typicode" }
}
```

### To run this container looks like:
```
docker run -d \
      -p 80:3000  -v {pwd}:/data  \
      demotascha/json-server
```