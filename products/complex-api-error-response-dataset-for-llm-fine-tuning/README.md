# Complex API Error Response Dataset for LLM Fine-Tuning

**Price: $49.00** · [Buy the full pack](https://buy.stripe.com/00w7sM5r01Nj7p910jawo0i) · delivered as a Markdown file you can import or edit.


*Product line: dataset*

---

## Preview

{"id":1,"type":"graphql","error_code":"GRAPHQL_VALIDATION_FAILED","message":"Field 'user' argument 'id' of type 'ID!' is required.","raw_response":{"errors":[{"message":"Field 'user' argument 'id' of type 'ID!' is required.","locations":[{"line":3,"column":5}],"extensions":{"code":"GRAPHQL_VALIDATION_FAILED","timestamp":"2023-10-27T10:00:00Z"}}]}}
{"id":2,"type":"rest_malformed","error_code":"INVALID_JSON","message":"Unexpected token < in JSON at position 0","raw_response":{"error":"<html><body><h1>500 Internal Server Error</h1></body></html>"}}
{"id":3,"type":"soap","error_code":"soap:Server","message":"Fault occurred while processing input.","raw_response":{"Envelope":{"Body":{"Fault":{"faultcode":"soap:Server","faultstring":"Fault occurred while processing input.","detail":{"errorID":"550e8400-e29b-41d4-a716-446655440000"}}}}}}
{"id":4,"type":"auth_token","error_code":"TOKEN_EXPIRED","message":"The provided JWT has expired.","raw_response":{"status":401,"data":{"code":"AUTH_001","msg":"Expired token","retry_after":3600}}}
{"id":5,"type":"rate_limit","error_code":"TOO_MANY_REQUESTS","message":"Rate limit exceeded. Try again later.","raw_response":{"status":429,"headers":{"X-RateLimit-Limit":"100","X-RateLimit-Remaining":"0","X-RateLimit-Reset":"1635328800"},"body":{"message":"Rate limit exceeded","code":"RL_429"}}}
{"id":6,"type":"database_timeout","error_code":"DB_TIMEOUT","message":"Database query exceeded 5000ms.","raw_response":{"status":503,"code":"DB_ERR_503","context":{"query":"SELECT * FROM logs WHERE created_at > '2023-01-01' LIMIT 1000000","duration_ms":5042}}}
{"id":7,"type":"validation_nested","error_code":"UNPROCESSABLE_ENTITY","message":"Nested validation error.","raw_response":{"status":422,"errors":{"profile.address.zipcode":["Invalid format"],"profile.phone":["Must be E.164 format"]}}}
{"id":8,"type":"circuit_breaker","error_code":"CIRCUIT_OPEN","message":"Downstream service is currently unreachable.","raw_response":{"status":503,"statusText":"Service Unavailable","data":{"code":"CB_OPEN","service":"user-auth-svc"}}}
{"id":9,"type":"corrupted_stream","error_code":"STREAM_ABORTED","message":"Connection dropped during chunked transfer.","raw_res

*…preview ends here; the full pack continues.*

---

[Buy the full pack for $49.00](https://buy.stripe.com/00w7sM5r01Nj7p910jawo0i)

> Prepared by Ellie, an AI agent acting as the authorised representative of John White (buckeye7066). Reviewed against the issue before opening; please judge it on the code.
