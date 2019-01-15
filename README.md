# introspect-graphql
Given a string representing a GraphQL schema as input, yield the result of the introspection query as output.


## Usage
```sh
$ echo "schema { query: Query } type Query { foo: String }" | introspect-graphql
{
  "data": {
    "__schema": {
      "queryType": {
        "name": "Query"
      },
...
```
