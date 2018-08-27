{
  "info": {
    "name": "Bitly Domains API Get Link Clicks",
    "_postman_id": "4d767056-d088-49a5-8e6c-cc0e31a7e26d",
    "description": "Returns entries from a user's link history in reverse chronological order.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Shorten",
      "item": [
        {
          "id": "571b3697-ef43-48e7-b279-30ddb8cbeb74",
          "name": "Get_shorten_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/shorten?domain=%7B%7D&format=%7B%7D&longUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a long URL, returns a bitly short URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71ffe1bf-fe7f-439b-b634-078c55c40489"
            }
          ]
        }
      ]
    },
    {
      "name": "Expand",
      "item": [
        {
          "id": "6a9151ce-d2ba-4432-92ea-338442ee2c24",
          "name": "Get_expand_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/expand?format=%7B%7D&hash=%7B%7D&shortUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a bitly URL or hash (or multiple), returns the target (long) URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33040dae-37e2-4121-9a1c-58423b1bfc17"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "bf54e027-ff13-428f-9692-1023ad326db2",
          "name": "Get_lookup_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/lookup?format=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This is used to query for a bitly link based on a long URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "574ca18e-8681-4a23-a36f-b3849a1999a0"
            }
          ]
        },
        {
          "id": "6af30d5c-6e26-4c25-8c3c-34bf380d88c2",
          "name": "Get_link_clicks_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/clicks?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns entries from a user's link history in reverse chronological order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b6e62882-d71c-4e0a-8877-8492b7747e20"
            }
          ]
        }
      ]
    },
    {
      "name": "Info",
      "item": [
        {
          "id": "801bc06d-6abd-48e2-bd9f-c3c273676aa7",
          "name": "Get_info_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/info?format=%7B%7D&hash=%7B%7D&shortUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This is used to return the page title for a given bitly link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da27d929-74d1-4e9e-9997-da71471c3949"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "0fc890e8-5679-47c3-9d4f-772a7793ede5",
          "name": "Get_user_info_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/user/info?format=%7B%7D&login=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return information about a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "389d656c-c157-41cb-a4f4-7f98797a8311"
            }
          ]
        },
        {
          "id": "edeca12b-cf3c-4dad-b347-90a1a337200e",
          "name": "Get_user_link_history_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/user/link_history?created_after=%7B%7D&created_before=%7B%7D&format=%7B%7D&limit=%7B%7D&user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns entries from a user's link history in reverse chronological order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "336d3340-ec61-407c-b36e-8d64c16e95fd"
            }
          ]
        },
        {
          "id": "a9ecc911-0740-4d9b-82f6-27678fe59465",
          "name": "Get_user_popular_links_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/user/popular_links?format=%7B%7D&limit=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the authenticated user's most-clicked bitly links (ordered by number of clicks) in a given time period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d76bc58-5ef0-43b4-9216-022a451c1c7a"
            }
          ]
        }
      ]
    }
  ]
}