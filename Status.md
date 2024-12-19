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

## POST /analyseExercise

Request

```json
{
  "uid":12345,
  "file": file,
  "exercise": ""
}
```

Response

```json
{
  "status": "success",
  "data": {
    "progress": "in queue"
  }
}
```

## GET /getExercise/12345

Response

```json
{
  "status": "success",
  "data": {
    "exerciseList": [
      {
        "name": "Broad Jump",
        "status": "Completed",
        "report": {
          "jump_distance": 5,
          "unit": "ft"
        }
      },
      {
        "name": "Squats",
        "status": "Completed",
        "report": {
          "reps": 34,
          "unit": "count"
        }
      },
      {
        "name": "Pull Ups",
        "status": "In Progress"
      },
      {
        "name": "Sit Ups",
        "status": "Not Started"
      },
      {
        "name": "Vertical Jump",
        "status": "Not Started"
      }
    ]
  }
}
```
