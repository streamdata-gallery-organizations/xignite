{
  "info": {
    "name": "Xignite Releases Get Historical Security Headlines",
    "_postman_id": "9daeb69e-1c0d-472c-8544-d1eee6aa4781",
    "description": "Returns headlines for a company and a date range.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Market Data",
      "item": [
        {
          "id": "b3d647b3-ef25-40e1-b453-c7a28f563a89",
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
              "id": "b61a718f-21f3-45ad-8e44-452a39f508de"
            }
          ]
        },
        {
          "id": "a38d3c23-f3f8-476d-a82b-ff0f75dcb60f",
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
              "id": "05662ba3-51e2-4dff-af24-0638decbb53f"
            }
          ]
        }
      ]
    }
  ]
}