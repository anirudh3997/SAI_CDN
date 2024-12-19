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

## GET /getStudents

Response

```json
{
  "status": "success",
  "data": {
    "athletesList": [
        {
            "uid": 12345
            "name":"Anirudh",
            "gender": "Male",
            "dob": "03/09/1997",
            "height": 160,
            "weight": 87
        },
        {
            "uid": 12346
            "name":"Animesh",
            "gender": "Male",
            "dob": "02/12/1997",
            "height": 159,
            "weight": 120
        },
        {
            "uid": 12347
            "name":"Vardhan",
            "gender": "Male",
            "dob": "02/12/1997"
        }
    ]
  }
}
```
