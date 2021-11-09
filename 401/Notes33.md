# GraphQL @connection

## Add relationships between types

we use `@connection` annotation to specify relationships between models `@model` like **many-to-many** relationships (by using using two **one-to-many** connections).

**GraphQL realationship**:

1. one-to-one connection: Example for one-to-one connection:

```type Project @model {
  id: ID!
  name: String
  team: Team @connection
}

type Team @model {
  id: ID!
  name: String!
}
```

2. one-to-many: Example for one-to-many:

```
type Post @model {
  id: ID!
  title: String!
  comments: [Comment] @connection(keyName: "byPost", fields: ["id"])
}

type Comment @model
  @key(name: "byPost", fields: ["postID", "content"]) {
  id: ID!
  postID: ID!
  content: String!
}
```

3. many-to-many: You can implement many to many using two 1-M `@connections`, an `@key`, and a joining `@model`.

 Example for many-to-many:

```
any to many using two 1-M @connections, an @key, and a joining @model. For example:

type Post @model {
  id: ID!
  title: String!
  editors: [PostEditor] @connection(keyName: "byPost", fields: ["id"])
}

# Create a join model and disable queries as you don't need them
# and can query through Post.editors and User.posts
type PostEditor
  @model(queries: null)
  @key(name: "byPost", fields: ["postID", "editorID"])
  @key(name: "byEditor", fields: ["editorID", "postID"]) {
  id: ID!
  postID: ID!
  editorID: ID!
  post: Post! @connection(fields: ["postID"])
  editor: User! @connection(fields: ["editorID"])
}

type User @model {
  id: ID!
  username: String!
  posts: [PostEditor] @connection(keyName: "byEditor", fields: ["id"])
}

```
So `many-to-many` connection needs two `@key`