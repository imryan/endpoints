## Insomnia Cookies endpoints
[insomniacookies.com](https://insomniacookies.com)

Get real-time UV Index by location. Optional altitude, ozone level and datetime could be provided.

## Real-time driver location
`GET https://insomniacookies.com/tracker/getDriverLocation/{order_id}`

Response:
```
{
  "status": {
    "status": "d",
    "reason": "",
    "store_lat": "40.7369205",
    "store_lng": "-74.0302510",
    "storeID": 1143,
    "store_name": "Hoboken - delivering to Hoboken and surrounding area",
    "shipping_address_1": "1 Castle Point Terrace",
    "shipping_address_2": "",
    "shipping_city": "Hoboken",
    "shipping_state": "NJ",
    "shipping_postcode": "07030"
  },
  "location": []
}
```
