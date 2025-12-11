# Troubleshooting

This page lists common issues and how to resolve them.

## Invalid API key

If you receive `401 Unauthorized`:

- Check that the key value is correct.
- Confirm that the key has not expired or been revoked.
- Verify that you are sending the key in the `Authorization: Bearer` header.

## No results

If a query returns no results:

- Make sure the track or ID exists in your catalog.
- Try lowering filters or constraints.
- Check that the correct environment (staging vs production) is used.

## Slow responses

If requests are slower than expected:

- Measure network latency between your servers and the AIMS API.
- Ensure you reuse HTTP connections where possible.
- Investigate whether you are sending very large files or complex filters.

## Rate limit exceeded

If you receive `429 Too Many Requests`:

- Implement exponential backoff and retries.
- Consider batching requests where appropriate.
- Contact support if you consistently hit rate limits.

If the issue persists, gather request IDs and timestamps and contact AIMS support with a short description of the problem.
