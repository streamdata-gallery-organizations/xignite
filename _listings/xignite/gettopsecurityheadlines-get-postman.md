{
  "info": {
    "name": "Xignite Releases Get Top Security Headlines",
    "_postman_id": "c6636a53-9e06-4b76-8011-63acffd16fbf",
    "description": "Returns a given number of company headlines published most recently.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Market Data",
      "item": [
        {
          "id": "35d0f08d-c59d-4bf4-9eb8-ba99ce8c3791",
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
              "id": "879af6f6-167a-4f39-8e3a-bfaf1881231d"
            }
          ]
        },
        {
          "id": "0a97e7bf-227a-4525-bca8-eca1064a5087",
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
              "id": "cbfbe6d9-72c8-4a12-b168-9ed36f88dea0"
            }
          ]
        },
        {
          "id": "2544ed80-a621-49af-8279-58fb34afedea",
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
              "id": "c87f047f-6812-44e2-9c6d-06643b44230f"
            }
          ]
        },
        {
          "id": "cbf4471b-c632-45c1-a3ad-74de1c647b94",
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
              "id": "b929520d-af09-4125-93f9-f3f5d9ce8ae5"
            }
          ]
        },
        {
          "id": "a8e1d1f5-6f11-4e50-b88a-3b90c10d891d",
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
              "id": "6b37d8e6-91a7-4f27-ac99-53c6b077476b"
            }
          ]
        },
        {
          "id": "171659a2-a024-4391-939b-e77b750958e8",
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
              "id": "459112c9-50ad-44ef-bb1e-ebc1479594a4"
            }
          ]
        },
        {
          "id": "076f4d86-b864-4a10-96ca-f38ef6ed73af",
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
              "id": "43aa8c9f-7b75-4579-beaa-6c763e557d2d"
            }
          ]
        },
        {
          "id": "19148290-2a62-4ab7-8b7b-15fff4833266",
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
              "id": "80bdaf33-2d27-45d1-a590-8c871bf88c6b"
            }
          ]
        }
      ]
    }
  ]
}