## Demo docker

### Backend - Books service

| Name           | Method | Path         |
|----------------|--------|--------------|
| Create book    | POST   | `/books`     |
| List all books | GET    | `/books`     |
| Get book by id | GET    | `/books/:id` |
| Remove book    | DELETE | `/books/:id` |

### Backend - News service

| Name                           | Method | Path            |
|--------------------------------|--------|-----------------|
| Create a news                  | POST   | `/api/news`     |
| List all news                 | GET    | `/api/news`     |
| Retrieve all News              | GET    | `/api/news/:id` |
| Retrieve a single News with id | PUT    | `/api/news/:id` |
| Delete a News with id          | DELETE | `/api/news/:id` |


`go mod tidy`

`go mod download`

`go run main.go`

`docker build -t books-service . `

`docker run -d -p 8080:8080 -v $(pwd)/db/:/app/db books-service`

`docker ps`

`docker logs NAMES`
