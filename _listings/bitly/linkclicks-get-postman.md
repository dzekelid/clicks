{
  "info": {
    "name": "Bitly Link Metrics API Link Clicks",
    "_postman_id": "958e3c48-b24b-4fd8-b4c0-4beee60491d3",
    "description": "Returns the number of clicks on a single Bitlink.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Link",
      "item": [
        {
          "id": "725ac208-0faa-487f-81d8-e814e8042489",
          "name": "linkClicks",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/clicks?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the number of clicks on a single Bitlink."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cb9068ab-8bfc-4950-9ba3-d90821c7ab4d"
            }
          ]
        }
      ]
    }
  ]
}