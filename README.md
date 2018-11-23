#### Run the example

```bash
git clone git@github.com:tancredi/swagger-examples-validation-demo.git
cd swagger-examples-validation-demo
npm install
npm start
```

The output should be an error looking like:

```
Swagger schema validation failed.
  Data does not match any schemas from 'oneOf' at #/paths//ping/get/responses/200
    Data does not match any schemas from 'oneOf' at #/paths//ping/get/responses/200/content/application/json/examples/Example2
      Additional properties not allowed: din at #/content/application/json/examples/Example2
      Missing required property: $ref at #/content/application/json/examples/Example2
    Missing required property: $ref at #/paths//ping/get/responses/200
```