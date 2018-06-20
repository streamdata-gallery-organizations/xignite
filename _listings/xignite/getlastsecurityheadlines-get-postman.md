{
  "info": {
    "name": "Xignite Releases Get Last Security Headlines",
    "_postman_id": "ebcb7aeb-1c75-40fd-8a92-36ac4e483868",
    "description": "Returns headlines for a company published since a specific date and time.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Market Data",
      "item": [
        {
          "id": "598586aa-6445-4cca-8814-0eed37cefc5e",
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
              "id": "b65af498-9495-47a9-967c-2805593fd88c"
            }
          ]
        },
        {
          "id": "57d59494-3ef1-4814-9a29-880fa906b416",
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
              "id": "03af04cf-9925-46ef-a7c1-39eadad17d21"
            }
          ]
        },
        {
          "id": "9952e480-c5cc-42b4-9b39-dc90c9d6983f",
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
              "id": "522353e8-8fab-4cf1-8ece-52971a3a4a38"
            }
          ]
        },
        {
          "id": "ffa16008-9bff-4166-a110-b1a13b9102ba",
          "name": "getGetlastsecurityheadlines",
          "request": {
            "url": "http://http://www.xignite.com//xReleases.xml/GetLastSecurityHeadlines/?Identifier=%7B%7D&IdentifierType=%7B%7D&SinceDate=%7B%7D&_Token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns headlines for a company published since a specific date and time."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1ad6ada-e8db-4e8c-af43-c60d9dca1bd2"
            }
          ]
        }
      ]
    }
  ]
}