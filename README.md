# Simple API Application

API backed by DynamoDB, deployed via GitHub Actions to AWS account 549725144537.

## Endpoints

- `GET /items` - List all items
- `POST /items` - Create item (body: `{"id": "123", "name": "example"}`)
- `GET /items/{id}` - Get specific item

## Local Testing

```bash
sam build
sam local start-api
```

## Deployment

Push to main branch triggers automatic deployment via GitHub Actions using ada credentials.
