## Token Data endpoints
[tokendata.io](https://www.tokendata.io)

The service just launched so be aware that these URLs may change in the future.
Also please remember to be respectful by not flooding the service with requests.

## Base URL
`https://www.tokendata.io`

## Token sales
`GET /icos`

Response:
```
{
  "data": [
    {
      "_id": "59667269d2bd9ca99ddfd54a",
      "name": "The Bancor Protocol",
      "ticker": "bancor",
      "whitepaper": "https://drive.google.com/file/d/0B3HPNP-GDn7aLXFWOFpTZEgyaEk/view",
      "description": "Platform to launch new tokens",
      "status": "Completed",
      "usd_raised": 153000000,
      "month": "Jun 2017",
      "start_date": 1497225600,
      "end_date": 1497225600,
      "current_token_price": 2.02843,
      "token_sale_price": 3.8566243,
      "token_return": 0.57,
      "website": "https://bancor.network/"
    },
 ...
}
```

## Advanced returns
`GET /icos/advanced`

Response:
```
{
  "data": [
    {
      "_id": "59667364d2bd9ca99ddfd64b",
      "name": "Populous",
      "ticker": "populous",
      "whitepaper": "http://www.populous.co/populous_whitepaper.pdf",
      "description": "Invoicing platform",
      "website": "http://www.populous.co/",
      "month": "Jun 2017",
      "start_date": 1496880000,
      "end_date": 1498262400,
      "usd_raised": 10842331.5,
      "num_tokens_sold": 36000000,
      "current_token_price": 2.43304,
      "token_sale_price": 0.3011759,
      "token_return": 7.6,
      "eth_return": 0.7,
      "btc_return": 0.88,
      "token_eth_return": 10.91,
      "token_btc_return": 8.64,
      "eth_sale_cmc": 323.7,
      "btc_sale_cmc": 2608.72
    },
 ...
}
```

## Upcoming ICOs
`GET /icos/upcoming`

Response:
```
{
  "data": [
    {
      "_id": "596ec501d2bd9ca99ddfdfeb",
      "name": "S3ntigraph",
      "website": "https://www.sentigraph.io/",
      "name_lower": "s3ntigraph",
      "whitepaper": "https://docs.wixstatic.com/ugd/743231_0b1030b0f6c64266bf0fec6605bfe945.pdf",
      "description": "Platform measuring sentiments & emotions",
      "status": "Planned",
      "month": "Aug 2017",
      "start_date": 1500508800,
      "end_date": 1501804800
    },
 ...
}
```
