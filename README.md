# jokes-service
A Jokes API with jokes searchable via query parameters

1. Run `npm install` to install your project dependencies. 
2. Testing is set up for you.  `npm run test` to run tests.  It is currently in watch-all mode.  This means it will run tests automatically after you save the index file.
3.  To test your endpoints using either a browser or Postman, you can run `npm run start-dev`.  This will run a local server for you (from the server.js file).
4. The API service needs to be set up for the following query parameters `content` and `tags` (ideally querying partial matches from the database).
5. TDD - Make red go green!




Example call:
```sh
$ curl -H "Accept: application/json" "http://localhost:4000/search?content=hipster&limit=2"
```

Example response
```json
{
  "results": [
    {
      "id": "GlGBIY0wAAd",
      "joke": "How much does a hipster weigh? An instagram."
    },
    {
      "id": "xc21Lmbxcib",
      "joke": "How did the hipster burn the roof of his mouth? He ate the pizza before it was cool."
    }
  ],
  "search_term": "hipster",
  "total_jokes": 2,
}
```