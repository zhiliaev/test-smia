# Getting started

This guide walks you through the basic setup and your first AIMS API request.

## Prerequisites

- An AIMS account.
- An API key with access to the Similarity Search API.
- Ability to make HTTPS requests from your server environment.

## Create an API key

1. Log into the AIMS dashboard.
2. Navigate to **API keys**.
3. Create a new key and store it securely.

## First request

```bash
curl https://api.aimsapi.com/v1/query/by-id \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{ "id": "track_123", "limit": 5 }'
```

You should receive a JSON response containing a list of similar tracks.

## Next steps

- Explore available endpoints in the **[API reference](./api-reference.md)**.
- Learn about search modes and parameters in **[Concepts](./concepts.md)**.
