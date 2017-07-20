# endpoints
Open source journal of URL digging with bonus web service.

## Accessing an endpoint
To access an endpoint:

`GET https://github.com/imryan/endpoints/blob/master/services` `// TODO`

Response:
```
{
  "services": [
    {
      "name": "tokendataio",
      "website": "https://www.tokendata.io",
      "documentation":"https://github.com/imryan/endpoints/docs/tokendataio",
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
  "documentation":"https://github.com/imryan/endpoints/docs/tokendataio",
  "endpoints": [
    "https://www.tokendata.io/icos",
    "https://www.tokendata.io/icos/advanced",
    "https://www.tokendata.io/icos/upcoming"
  ]
  ...
}
```

## Contributions
I encourage everyone to throw in anything cool they find scraping the web. Project will be updated regularly.
