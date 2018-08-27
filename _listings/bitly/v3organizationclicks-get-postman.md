{
  "info": {
    "name": "Bitly Organization Metric API Organization Clicks",
    "_postman_id": "b7d3d6f5-d879-423c-847e-edfe0db5ea4f",
    "description": "Returns the number of clicks on Bitlinks created by your organization or by other Bitly users that point to your domains.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organization",
      "item": [
        {
          "id": "113bb84d-4733-44c2-9aae-5973dac63a99",
          "name": "organizationBrandMessages",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/organization/brand_messages?domain=%7B%7D&limit=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the top Bitlinks created by you with traffic, that did not also have non-organization traffic in the same time period, ordered by clicks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bf8a46c-8a0d-4c7c-a965-d92db0d1335c"
            }
          ]
        },
        {
          "id": "7547a41f-ae04-4ebc-a084-a5d1f855f5c4",
          "name": "organizationClicks",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/organization/clicks?domain=%7B%7D&limit=%7B%7D&login=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the number of clicks on Bitlinks created by your organization or by other Bitly users that point to your domains."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9d457bf-5a7c-4b51-b9af-98af114cb740"
            }
          ]
        }
      ]
    }
  ]
}