This is an effort to document REST++ API for TigerGraph database using OpenAPI 3.x specification.

The original API documentation is located here: https://docs.tigergraph.com/tigergraph-server/current/api/intro

## Showing the API documentation
The API specification can be used to generate the API documentation.

One easy way to browse through the API is using [Swagger UI](https://swagger.io/):

```bash
docker run -d -p 8080:8080 -e SWAGGER_JSON=/api.yaml -v $PWD/restpp.api.yaml:/api.yaml swaggerapi/swagger-ui
```
_Note: This assumes that the specification you want to see is placed in the current directory and
is named 'restpp.api.yaml'.

Another convenient way is to use [Swagger Inspector](https://inspector.swagger.io/).

## Project details
This folder contains:

|                     |                                                                                                                                           |
|---------------------|-------------------------------------------------------------------------------------------------------------------------------------------|
| restpp.api.old.yaml | OpenAPI specification converted from [Postman collection](https://github.com/TigerGraph-DevLabs/TigerGraph-Postman) I found on the web.   |
| restpp.api.yaml     | Target version of the specification that I work on from scratch.                                                                          |

I hope to use the specification to generate Java client for REST++ API.
