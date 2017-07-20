# endpoints
Open source journal of URL digging with bonus web service.

## Accessing an endpoint
To access an endpoint:

`GET https://raw.githubusercontent.com/imryan/endpoints/master/services.json`

Response:
```
{
  "services": [
    {
      "name": "tokendataio",
      "website": "https://www.tokendata.io",
      "documentation":"https://raw.githubusercontent.com/imryan/endpoints/master/docs/tokendataio.md",
      "endpoints": [
        "https://www.tokendata.io/icos",
        "https://www.tokendata.io/icos/advanced",
        "https://www.tokendata.io/icos/upcoming"
      ]
    }
  ]
}
```

## Service model
```
{
  "name": "tokendataio",
  "website": "https://www.tokendata.io",
  "documentation":"https://raw.githubusercontent.com/imryan/endpoints/master/docs/tokendataio.md",
  "endpoints": [
    "https://www.tokendata.io/icos",
    "https://www.tokendata.io/icos/advanced",
    "https://www.tokendata.io/icos/upcoming"
  ]
}
```

## Contributions
I encourage everyone to throw in anything cool they find scraping the web. Project will be updated regularly.
