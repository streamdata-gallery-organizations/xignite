{
  "info": {
    "name": "Xignite Releases Search Market Headlines",
    "_postman_id": "54ad6d96-0f0a-4355-8234-a5541a691f96",
    "description": "Search market headlines across all companies based on date, source, and title.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Market Data",
      "item": [
        {
          "id": "361204d5-b855-45c2-8d7d-ccb6c138ba63",
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
              "id": "33c29f6a-fa24-4107-986e-cc69f97b6864"
            }
          ]
        },
        {
          "id": "6b6757d6-9cf4-470f-93f6-bd2d991941e4",
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
              "id": "b91ab817-d4ad-414b-bebd-0459fc8fde6e"
            }
          ]
        },
        {
          "id": "56bb9c1a-533f-4441-8dad-cb30d136cb77",
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
              "id": "79f3f427-a686-4efd-a250-f9814ff63549"
            }
          ]
        },
        {
          "id": "ca828cc6-bc8d-4ed9-b1a9-27c68c971aaa",
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
              "id": "702584f0-1a4f-462e-ad8a-bfcd32f5018d"
            }
          ]
        },
        {
          "id": "61b90889-4d3e-4981-a2eb-3d2ffbb5e4a2",
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
              "id": "b1544499-93a5-449e-b0df-27311e130ae0"
            }
          ]
        },
        {
          "id": "5ab3a27b-1368-4269-9fc0-acc67f3b74ca",
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
              "id": "a96f524a-f561-41e6-9da5-7fb5e5e8d949"
            }
          ]
        },
        {
          "id": "114483e5-0c9e-4461-a8e2-9413545ecf37",
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
              "id": "76167e4f-00a8-4296-aa0d-3f501ee87621"
            }
          ]
        },
        {
          "id": "97f32269-a504-48c4-8d32-14007e2b1e77",
          "name": "getGettopsecurityheadlines",
          "request": {
            "url": "http://http://www.xignite.com//xReleases.xml/GetTopSecurityHeadlines/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a given number of company headlines published most recently."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1bc5c214-2bb4-4fd4-9275-00df3dcf4c30"
            }
          ]
        },
        {
          "id": "49bfc3dc-9408-489a-8fda-4c1a4a5fee7c",
          "name": "getSearchmarketheadlines",
          "request": {
            "url": "http://http://www.xignite.com//xReleases.xml/SearchMarketHeadlines/?EndDate=%7B%7D&Source=%7B%7D&StartDate=%7B%7D&Title=%7B%7D&_Token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search market headlines across all companies based on date, source, and title."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9eff3a39-b428-481d-94ed-7823f1b34cda"
            }
          ]
        }
      ]
    }
  ]
}