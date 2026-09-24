curl -X POST https://sandbox-api.polygon.technology/v0.13/customers \
  -H "Authorization: Bearer {accessToken}" \
  -H "Content-Type: application/json" \
  -H "Idempotency-Key: cst-first-customer-001" \
  -d '{
    "type": "individual",
    "firstName": "josphine",
    "lastName": "kiarie",
    "email": "josphinekiarie47@gmail.com",
    "phone": "+254741791814",
    "birthDate": "1971/09/01",
    "nationality": "kenyan",
    "residentialAddress": {
      "line1": "kamiti rd zimmerman",
      "city": "Nairobi",
      "country": "kenya",
      "zipCode": "00100"
    },
    "identifyingInformation": [
      { "type": "ssn", "issuingCountry": "kenya", "number": "" }
    ],
    "endorsements": ["basic", "cryptoCustody", "usd"]
  }'
