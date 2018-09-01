{
  "info": {
    "name": "Xignite Releases Get Release Content",
    "_postman_id": "afbe0843-4d15-443d-8893-e5a24185fd88",
    "description": "Return detailed information about a release as well as its content.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Market Data",
      "item": [
        {
          "id": "34039b93-edf1-4c1a-b236-9687540182f8",
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
              "id": "a01ec0df-f0c6-4fbf-9317-4534a01487f9"
            }
          ]
        },
        {
          "id": "b81ef289-6a21-4798-bc03-e7e365d7f231",
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
              "id": "79702e91-0e00-4bbe-96f5-3b2422613d07"
            }
          ]
        },
        {
          "id": "821e3109-e97d-41db-905e-3cbeeaab32d1",
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
              "id": "a32475a7-2eea-4163-b1fa-094da7fa8f8c"
            }
          ]
        },
        {
          "id": "d258711e-ce75-41d9-9cde-5961576d4e71",
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
              "id": "9d45c9f6-7f4c-468a-a09a-029dfc61b29c"
            }
          ]
        },
        {
          "id": "da47f43b-b7af-457c-ada4-0161b29c4a3c",
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
              "id": "a9571929-5172-4801-9910-cd3f6cefdb43"
            }
          ]
        }
      ]
    }
  ]
}