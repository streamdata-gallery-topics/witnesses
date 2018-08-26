{
  "info": {
    "name": "Steem get_witnesses",
    "_postman_id": "1437504d-660c-4911-8e76-050ba98610cd",
    "description": "get_witnesses",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "bdd32d46-f111-462e-a47c-55feb1b90c4a",
          "name": "get-witnesses",
          "request": {
            "url": "http://api.steemjs.com/get_witnesses?witnessIds=%7B%7D",
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
            "description": "get_witnesses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2241f93-fc31-4004-b146-c353c2edb705"
            }
          ]
        }
      ]
    }
  ]
}