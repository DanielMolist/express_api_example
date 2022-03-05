# Express API example
Basic example of how to create a REST API with Express (No database connection)

## Installation & Local Run
Ensure you have node 16 or higher.

1. `git clone https://github.com/DanielMolist/express_api_example.git`
2. `cd express_api_example`
3. `npm install`
4. `npm start`

## API Call
### Local:
#### Get all notes
```
curl -X GET http://localhost:3001/api/notes
```
#### Get note by id
```
curl -X GET http://localhost:3001/api/notes/1
```
#### Create new note
```
curl -X POST http://localhost:3001/api/notes
```
- Header:
```
Content-Type:application/json  
```
- Body:
```json
{
    "content": "I am creating a new note",
    "important": false
}
``` 

#### Delete note by id
```
curl -X DELETE http://localhost:3001/api/notes/1
```

### Response
```json
{
    "id": 1,
    "content": "HTML is easy",
    "date": "2019-05-30T17:30:31.098Z",
    "important": true
}
``` 
