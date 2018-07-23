# gqlgen-test
Test Golang gqlgen GraphQL Framework

### Skills
1. golang
2. GraphQL
3. gqlgen


Build  
```
  > dep ensure
  > go get github.com/vektah/gorunpkg
  > go generate ./... (gqlgen if install gqlgen by go get -u github.com/vektah/gqlgen)
  > go run main.go
```

```
mutation createTodo {
  createTodo(input:{text:"todo", user:"1"}) {
    user {
      id
    }
    text
    done
  }
}

query findTodos {
  	todos {
      text
      done
      user {
        name
      }
    }
}
```
