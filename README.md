# GraphQL
GraphQL

### 
Open
localhost:5000/graphql

###
```
query {
	books
}
```

###
Query books
```
{
	books
}
```

###
Query Authors
```
{
	authors {
	  id
    name
	}
}
```

###
Query authors and their books
```
{
	authors {
	  id
    name
		books {
      name
    }
	}
}
```

###
Get specific Book
```
{
  book(id: 1) {
		name
  }
}
```

###
Get specific author
```
{
	author(id: 1) {
		name
	}
}
```

###
Add book
```
mutation {
  addBook(name: "New Name", authorId: 1) {
    id
    name
  }
}
```

###
Add authors
```
mutation {
	addAuthor(name: "New Author") {
		id
    name
	}
}
```
