## POST /register

Request

```json
{
  "name": "Anirudh",
  "gender": "Male",
  "dob": "03/09/1997"
}
```

Response

```json
{
  "status": "success",
  "data": {
    "uid": 12345
  }
}
```

## POST /height

Request

```json
{
  "uid":12345,
  "image": file
}
```

Response

```json
{
  "status": "success",
  "data": {
    "uid": 12345
    "name":"Anirudh",
    "gender": "Male",
    "dob": "03/09/1997",
    "height": 157
  }
}
```

## POST /setHeight

Request

```json
{
  "uid": 12345,
  "height": 160,
  "weight": 87
}
```

Response

```json
{
  "status": "success",
  "data": {
    "uid": 12345
    "name":"Anirudh",
    "gender": "Male",
    "dob": "03/09/1997",
    "height": 160,
    "weight": 87
  }
}
```

## GET /setHeight
