# Invoice

## Retrieve your invoices

{% $api_token %}

```bash
curl -X 'GET' \
  'https://api.hypeproxy.dev/v3/invoices' \
  -H 'accept: application/json' \
  -H 'Authorization: Bearer {% $api_token %}'
```