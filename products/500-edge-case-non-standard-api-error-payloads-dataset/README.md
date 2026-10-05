# 500+ Edge-Case & Non-Standard API Error Payloads Dataset

**Price: $29.99** · [Buy the full pack](https://buy.stripe.com/7sYeVebPo8bH7p924nawo0p) · delivered as a Markdown file you can import or edit.


*Product line: dataset*

---

## Preview

{"id": 1, "type": "OAuth-Malformed-Grant", "status": 400, "payload": {"error": "invalid_grant", "error_description": "The provided authorization grant is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client.", "trace_id": "req_9a8b7c6d5e"}}
{"id": 2, "type": "GraphQL-Depth-Limit-Exceeded", "status": 429, "payload": {"errors": [{"message": "Query depth limit exceeded. Maximum allowed: 5, requested: 8.", "extensions": {"code": "DEPTH_LIMIT_EXCEEDED"}}]}}
{"id": 3, "type": "Rate-Limit-Retry-After-Missing", "status": 429, "payload": {"error": "Too Many Requests", "message": "Rate limit exceeded. Please wait before retrying.", "retry_after": null}}
{"id": 4, "type": "SOAP-Fault-Version-Mismatch", "status": 500, "payload": {"faultcode": "soap:VersionMismatch", "faultstring": "The version of the SOAP protocol specified is not supported.", "detail": {"ns2:SupportedVersions": ["1.1", "1.2"]}}}
{"id": 5, "type": "Stripe-Idempotency-Conflict", "status": 409, "payload": {"error": {"message": "Idempotency key 'key_12345' was used with a different request.", "type": "idempotency_error"}}}
{"id": 6, "type": "AWS-S3-Signature-Does-Not-Match", "status": 403, "payload": {"Code": "SignatureDoesNotMatch", "Message": "The request signature we calculated does not match the signature you provided. Check your key and signing method.", "RequestId": "F66750033B6C98F8"}}
{"id": 7, "type": "Content-Type-Mismatched", "status": 415, "payload": {"error": "Unsupported Media Type", "details": "Expected application/json, got text/plain."}}
{"id": 8, "type": "Database-Connection-Timeout", "status": 504, "payload": {"code": "ETIMEDOUT", "message": "Database cluster 'db-cluster-01' failed to respond within 3000ms."}}
{"id": 9, "type": "Circuit-Breaker-Open", "status": 503, "payload": {"error": "Service Unavailable", "message": "Circuit breaker is OPEN for service 'auth-provider'. Failing fast.", "circuit": "auth-provider-cb"}}
{"id": 10, "type": "JSON-Pointer-Invalid", "status": 400, "payload": {"error": "Invalid JSON Pointer", "pointer": "/nonexistent/key", "reason": "Reference not found."}}
...[content truncated for brevi

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $29.99](https://buy.stripe.com/7sYeVebPo8bH7p924nawo0p)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
