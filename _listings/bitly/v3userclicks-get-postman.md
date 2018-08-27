{
  "info": {
    "name": "Bitly User Metrics API User Clicks",
    "_postman_id": "ee2a7a37-de2a-45bc-9358-de4db721f78b",
    "description": "Returns the aggregate number of clicks on all of the authenticated users Bitlinks.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "8834a100-83be-4db1-80c9-b72c92d4a419",
          "name": "userClicks",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/user/clicks?format=%7B%7D&limit=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the aggregate number of clicks on all of the authenticated users Bitlinks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6d18326-264e-40a7-bc36-134e3acabcf1"
            }
          ]
        }
      ]
    }
  ]
}