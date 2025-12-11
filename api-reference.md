# API reference

This page lists the core AIMS API endpoints used for similarity search and related features.

## Authentication

All requests must include a bearer token:

```bash
-H "Authorization: Bearer YOUR_API_KEY"
```

Never expose your API key in client-side code or logs.

## Search by ID

`POST /v1/query/by-id`

Use this endpoint when you already know the internal AIMS track ID.

Important parameters:

- `id` – required, the query track ID.
- `limit` – maximum number of results to return.

## Search by file

`POST /v1/query/by-file`

Upload the audio file directly:

- Send as `multipart/form-data`.
- The file should be in a supported audio format.

## Autocomplete

`POST /v1/autocomplete`

Retrieve suggestions for metadata or prompt text.

Common parameters:

- `query` – the partial input from the user.
- `limit` – maximum number of suggestions.

## Error handling

The API returns standard HTTP status codes:

- `400` – invalid request.
- `401` – authentication failed.
- `429` – rate limit exceeded.
- `500` – internal server error.

See **[Troubleshooting](./troubleshooting.md)** for more details.
