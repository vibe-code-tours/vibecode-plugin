---
name: API Design
description: Use when designing REST/HTTP endpoints — resource naming, status codes, errors, pagination, a consistent response envelope.
version: 1.0.0
---

# API Design

Predictable APIs are easy to use and easy to debug.

## Resources & methods
- Nouns, plural: `/users`, `/users/{id}/orders`. No verbs in paths.
- `GET` read, `POST` create, `PUT/PATCH` update, `DELETE` remove. Don't `GET` something that mutates.

## Status codes
- `200` ok, `201` created, `204` no content, `400` bad input, `401` no auth, `403` forbidden, `404` missing, `409` conflict, `422` validation, `429` rate-limited, `500` server.

## Response envelope (be consistent)
```json
{ "success": true, "data": { }, "error": null, "meta": { "page": 1, "total": 42 } }
```
On error: `success:false`, `data:null`, `error:"clear message"`. Never leak stack traces.

## Always
- Validate input at the boundary. Reject early with a clear message.
- Paginate lists (`page`/`limit` or cursor). Never return unbounded arrays.
- Version when you break: `/v1/...`.
