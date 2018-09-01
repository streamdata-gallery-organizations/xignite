{
  "info": {
    "name": "Xignite Releases Get Top Market Headlines",
    "_postman_id": "07105592-b567-4e69-9755-14ca24fcfc59",
    "description": "Returns a given number of market headlines published most recently.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Market Data",
      "item": [
        {
          "id": "3e92f7fc-0a61-435c-9aaf-5403bffcb925",
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
              "id": "6c0af5dc-ae83-4a9d-9c9a-dca36b3c8833"
            }
          ]
        },
        {
          "id": "836e2e26-0c7e-416c-a323-e22ed1aec3fc",
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
              "id": "ca9a1643-b946-495a-801c-c36a7a5aaf01"
            }
          ]
        },
        {
          "id": "2f8a8b78-297b-47c3-ae3c-e7fc2104b0d7",
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
              "id": "6c22f419-909e-4620-bd6e-a34b0a85a3bf"
            }
          ]
        },
        {
          "id": "7c808c78-5c73-498f-bfcd-bf2b6e8fed21",
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
              "id": "71f40c08-3f5e-406f-8ff3-6d4273c12d2b"
            }
          ]
        },
        {
          "id": "540b5468-6391-472b-a30f-7855c68e0f88",
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
              "id": "327210a8-998c-4b39-b472-4d99004732bd"
            }
          ]
        },
        {
          "id": "7e2b2281-f053-46cb-be9e-5ffe123b9104",
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
              "id": "ee7ae56f-1d49-450d-a4bd-396afe6add03"
            }
          ]
        },
        {
          "id": "3eda252f-210d-4516-ba1b-b204c8a763f9",
          "name": "getGettopmarketheadlines",
          "request": {
            "url": "http://http://www.xignite.com//xReleases.xml/GetTopMarketHeadlines/?Count=%7B%7D&_Token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a given number of market headlines published most recently."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9ffd8c5-8299-4615-ac41-7c9ee593b303"
            }
          ]
        }
      ]
    }
  ]
}