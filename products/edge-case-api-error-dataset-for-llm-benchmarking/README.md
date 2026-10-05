# Edge-Case API Error Dataset for LLM Benchmarking

**Price: $15.00** · [Buy the full pack](https://buy.stripe.com/8x26oIcTs8bHgZJdN5awo0s) · delivered as a Markdown file you can import or edit.


*Product line: digital_product*

---

## Preview

{"id": "EC-001", "category": "Authentication", "status_code": 401, "format": "JSON", "description": "Nested WWW-Authenticate challenge with multiple schemes", "response": {"error": "invalid_token", "message": "Token expired at 2026-09-01T12:00:00Z", "details": {"schemes": ["Bearer", "OAuth2"], "timestamp": "2026-09-01T12:01:00Z"}}}
{"id": "EC-002", "category": "GraphQL", "status_code": 200, "format": "JSON", "description": "GraphQL partial success with error array in extensions", "response": {"data": {"user": null}, "errors": [{"message": "User not found", "locations": [{"line": 2, "column": 3}], "path": ["user"], "extensions": {"code": "USER_NOT_FOUND", "retriable": false}}]}}
{"id": "EC-003", "category": "Rate Limiting", "status_code": 429, "format": "Custom Header", "description": "Standard 429 with non-standard Retry-After-Milliseconds header", "response": {"error": "Rate limit exceeded", "retry_after_ms": 4500}, "headers": {"X-RateLimit-Limit": "1000", "X-RateLimit-Remaining": "0", "Retry-After-Milliseconds": "4500"}}
{"id": "EC-004", "category": "Validation", "status_code": 422, "format": "JSON", "description": "Complex nested validation error with pointer references", "response": {"error": "Unprocessable Entity", "errors": [{"pointer": "/user/profile/address/zip", "code": "invalid_pattern", "message": "Zip code must be 5 digits"}, {"pointer": "/user/email", "code": "duplicate", "message": "Email already registered"}]}}
{"id": "EC-005", "category": "Gateway Timeout", "status_code": 504, "format": "HTML-in-JSON", "description": "Upstream proxy returns partial HTML error page disguised as JSON", "response": {"upstream_error": "<html><body><h1>504 Gateway Time-out</h1><p>The server didn't respond in time.</p></body></html>", "upstream_source": "auth-cluster-01"}}
{"id": "EC-006", "category": "Concurrency", "status_code": 409, "format": "JSON", "description": "Optimistic locking failure with conflict details", "response": {"error": "Conflict", "message": "The resource was modified by another request", "conflict_info": {"current_version": 12, "submitted_version": 10, "last_modified_by": "user_7788"}}}
{"id": "EC-007", "category": "SaaS-API", "status_code": 403,

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $15.00](https://buy.stripe.com/8x26oIcTs8bHgZJdN5awo0s)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
