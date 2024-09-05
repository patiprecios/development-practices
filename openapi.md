# Open api

The open api specification is located in the `openapi.yaml` file under docs folder of each repository exposing an web api. This file is used to generate the client and server code.

## Use the open api specification

You can use the open api specification in the following ways:

### Importing to Postman

You can import the open api specification to Postman. This will allow you to create automatically a collection of endpoints to test the API.

Follow steps in [this link](https://learning.postman.com/docs/getting-started/importing-and-exporting-data/#importing-data-into-postman) to import the open api specification to Postman.

### Using Swagger UI

You can use the open api specification to generate a Swagger UI:

```bash
docker run --rm -p 80:8080 -e SWAGGER_JSON=//assets/openapi.yml -v /${PWD}/docs/assets:/assets swaggerapi/swagger-ui
```

### Using ReDoc

You can use the open api specification to generate a ReDoc:

```bash
docker run --rm -p 80:80 -e SPEC_URL=assets/openapi.yml -v /$(PWD)/docs/assets:/usr/share/nginx/html/assets redocly/redoc
```

### Using VSCode extension

Install the [OpenAPI viewer extension](https://marketplace.visualstudio.com/items?itemName=42Crunch.vscode-openapi). Use the comand `OpenAPI: Show preview using swagger ui` to open the preview.
