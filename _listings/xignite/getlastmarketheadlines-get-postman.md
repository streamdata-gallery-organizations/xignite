{
  "info": {
    "name": "Xignite Releases Get Last Market Headlines",
    "_postman_id": "86da9a02-575c-4dad-b9a9-09414e4dcb8c",
    "description": "Returns market headlines published since a specific date and time.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Market Data",
      "item": [
        {
          "id": "7c1281de-910f-4e3f-bdf3-de4c21931078",
          "name": "getGethistoricalmarketheadlines",
          "request": {
            "url": "http://http://www.xignite.com//xReleases.xml/GetHistoricalMarketHeadlines/?EndDate=%7B%7D&Source=%7B%7D&StartDate=%7B%7D&_Token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns market headlines for a date range."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0c5eff0-b8ea-45f4-82f6-754f42cf05e0"
            }
          ]
        },
        {
          "id": "de2291f6-fb05-472b-8120-8cb996eaae72",
          "name": "getGethistoricalsecurityheadlines",
          "request": {
            "url": "http://http://www.xignite.com//xReleases.xml/GetHistoricalSecurityHeadlines/?EndDate=%7B%7D&Identifier=%7B%7D&IdentifierType=%7B%7D&Source=%7B%7D&StartDate=%7B%7D&_Token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns headlines for a company and a date range."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30de59ea-3c4f-407b-bc12-cb550f8c5e1a"
            }
          ]
        },
        {
          "id": "bf169d5f-b6ed-4123-ac5e-5a1e5b64de2a",
          "name": "getGetlastmarketheadlines",
          "request": {
            "url": "http://http://www.xignite.com//xReleases.xml/GetLastMarketHeadlines/?SinceDate=%7B%7D&_Token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns market headlines published since a specific date and time."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28467343-041c-4a9c-af49-a842a4b16b84"
            }
          ]
        }
      ]
    }
  ]
}