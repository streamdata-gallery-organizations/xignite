{
  "info": {
    "name": "Xignite Releases Get Historical Market Headlines",
    "_postman_id": "900e156f-3c97-4dad-a338-ca63ad5993ac",
    "description": "Returns market headlines for a date range.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Market Data",
      "item": [
        {
          "id": "059a2eac-c36f-44a2-a3ee-9fa2bac3091f",
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
              "id": "6999ebc6-1d41-4c2e-b73c-1bdc5db9b2e2"
            }
          ]
        }
      ]
    }
  ]
}