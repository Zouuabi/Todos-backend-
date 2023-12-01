# todo_app

# 1 Create a new todo
curl --request POST \
  --url http://localhost:8080/todos \
  --header 'Content-Type: application/json' \
  --data '{
  "title": "Take out trash"
}'

# 2 Read all todos 
curl --request GET \
  --url http://localhost:8080/todos

# 3 Read a specific todo by id
curl --request GET \
  --url http://localhost:8080/todos/<id>

# 4 Update a specific todo by id
curl --request PUT \
  --url http://localhost:8080/todos/<id> \
  --header 'Content-Type: application/json' \
  --data '{
  "title": "Take out trash!",
  "isCompleted": true
}'

# 5 Delete a specific todo by id
curl --request DELETE \
  --url http://localhost:8080/todos/<id>