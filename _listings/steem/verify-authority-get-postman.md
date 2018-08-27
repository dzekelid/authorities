{
  "info": {
    "name": "Steem verify_authority",
    "_postman_id": "db5ce1ce-60ee-45b9-a540-6214064ada20",
    "description": "verify_authority",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Verify",
      "item": [
        {
          "id": "aac232be-06b3-4286-b1dc-681dcf86bdbc",
          "name": "verify-authority",
          "request": {
            "url": "http://api.steemjs.com/verify_authority?trx=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "verify_authority"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "406dc66a-9da5-41f8-8944-e5cf5259b129"
            }
          ]
        }
      ]
    }
  ]
}