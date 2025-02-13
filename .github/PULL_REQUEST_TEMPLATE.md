## Description
Added a route `GET /api/v1/books/{book_id}` to get a single book from the API.<br>
The route will return a `404 ❌` if the book does not exist in the in-memory database.


## Related Task
[HNG12 Stage 2 Task](https://hng12.slack.com/archives/C088PK3KE2K/p1739195475622999)

## How Has This Been Tested?
- Ran `pytest` locally (and all passed)
- Personally tested invalid endpoints with thunderclient (eg. `/books/78`) to confirm 404 response

## Deployment
- Configured Nginx as a reverse proxy for the FastAPI application

## Final Notes
- Added `hng12-devbotops` as a collaborator
