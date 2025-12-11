# Concepts

This page explains the core concepts you will encounter when working with the AIMS API.

## Similarity search

AIMS compares a query track (or its ID) against your catalog and returns the most similar items.

Key ideas:

- **Query track** – the item you use as the basis for similarity.
- **Candidates** – items in your catalog that can be returned as results.
- **Score** – numeric measure of similarity between query and candidate.

## Highlights

Highlights allow you to identify the most relevant parts of a track.

- You can request highlights by setting `highlights: true`.
- The response then contains time ranges that AIMS considers most relevant.

## Segments

Segments let you define which part of a track to use for similarity:

- Use `time_offset` and `time_limit` in your request.
- The segment must be within the allowed duration limit.

## Autocomplete

Autocomplete provides suggestions for metadata, labels, or prompt text as the user types.

See **[API reference](./api-reference.md#autocomplete)** for request and response formats.
