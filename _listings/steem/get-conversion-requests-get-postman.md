{
  "info": {
    "name": "Steem get conversation",
    "_postman_id": "49d134aa-f848-4f12-bee2-0f7278ca9b36",
    "description": "get conversation requests of account",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "9de63bbc-8e8b-46d1-a9cb-88cd53fa113d",
          "name": "get-conversation-requests-of-account",
          "request": {
            "url": "http://api.steemjs.com/get_conversion_requests?accountName=%7B%7D",
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
            "description": "get conversation requests of account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01b84329-71cd-4b6d-93a3-0013b1a8b377"
            }
          ]
        }
      ]
    }
  ]
}