## Open UV endpoints
[openuv.io](https://www.openuv.io)

Get real-time UV Index by location. Optional altitude, ozone level and datetime could be provided.

## Base URL
`https://api.openuv.io/api/v1/uv`

## Real-time UV index
`GET https://api.openuv.io/api/v1/uv`

Parameters:
- `lat` : `'-33.34'`
- `lon` : `'115.342'`
- `dt`  : `'2018-01-24T10:50:52.283Z'`

Headers:
- `Content-Type` : `'application/json'`
- `X-Access-Token` : `'token'`

Response:
```
{
  "result":
  {
    "uv": 2.2375,
    "uv_time": "2018-02-04T18:22:50.838Z",
    "uv_max": 2.7507,
    "uv_max_time": "2018-02-04T17:11:20.725Z",
    "ozone": 296.3,
    "ozone_time": "2018-02-04T18:05:16.529Z"
  }
}
```
