---
"swagger-typescript-api": patch
---

fix: prioritize urlencoded content type

The previous logic would always default to multipart/form-data when a form was used. This change ensures that application/x-www-form-urlencoded is prioritized when it is present in the schema.
