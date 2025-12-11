# AIMS API Documentation

Welcome to the AIMS Similarity Search API docs.  
Here you can learn how to integrate, configure, and operate AIMS in your product.

Use the search bar at the top of the page to quickly jump to any topic.  
Start typing – you’ll see section-level suggestions and can click directly into the relevant part of the docs.

---

## Getting started

If you're new here, start with:

- [Quick start guide](./getting-started.md)
- [Concepts](./concepts.md)
- [API reference](./api-reference.md)
- [Troubleshooting](./troubleshooting.md)

---

## Quick start example

```bash
curl https://api.aimsapi.com/v1/query/by-id \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "id": "track_123",
    "limit": 10
  }'
```

---

## Typical integration flow

1. Ingest your catalog.
2. Configure similarity search behaviour.
3. Integrate the results into your product UI.
4. Track conversions and iterate based on analytics.

See **[Getting started](./getting-started.md)** for a step-by-step guide.
