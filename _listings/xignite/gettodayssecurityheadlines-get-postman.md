{
  "info": {
    "name": "Xignite Releases Get Todays Security Headlines",
    "_postman_id": "98d00820-2cda-4d33-8216-deab0eaf5013",
    "description": "Returns headlines for a company published today.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Market Data",
      "item": [
        {
          "id": "73a635b4-e6a8-4dfc-a626-44febaca15aa",
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
              "id": "502564a7-8b99-466a-910c-ae8ceae86fd1"
            }
          ]
        },
        {
          "id": "0750f892-428d-4330-92d3-1292b0dc3368",
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
              "id": "0f75bf48-909d-45d7-a2f8-6eb5672fce60"
            }
          ]
        },
        {
          "id": "9aba0d1f-b948-4483-99c9-81908dab6e85",
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
              "id": "cd0bbb56-e8e7-4b09-8802-eae78ead68e6"
            }
          ]
        },
        {
          "id": "62c31a67-6406-4f1f-8456-c20d31977a60",
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
              "id": "7dc661ed-c4c1-4606-b159-359b392b6b9e"
            }
          ]
        },
        {
          "id": "8c889d58-ccd3-4105-a3cc-46ab800edfc8",
          "name": "getGetreleasecontent",
          "request": {
            "url": "http://http://www.xignite.com//xReleases.xml/GetReleaseContent/?ReleaseID=%7B%7D&_Token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return detailed information about a release as well as its content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3026e5ec-6b20-4afe-adb3-7d922d68a392"
            }
          ]
        },
        {
          "id": "818be32a-7946-4cca-bb8d-516c7e62deea",
          "name": "getGettodayssecurityheadlines",
          "request": {
            "url": "http://http://www.xignite.com//xReleases.xml/GetTodaysSecurityHeadlines?Identifier=%7B%7D&IdentifierType=%7B%7D&_Token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns headlines for a company published today."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f72c5e6d-ec82-4684-b5b0-26469f889c20"
            }
          ]
        }
      ]
    }
  ]
}