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

## Order status
`GET https://insomniacookies.com/tracker/getOrderStatus`

Parameters:
- `trackingID` : `'779725445b8610e2'`

Response:
```
{
  "0": {
    "shipping_method": "4",
    "store_id": 1143,
    "id": 1988790659,
    "status": 6,
    "noteExist": 0
  },
  "store": {
    "name": "Hoboken - delivering to Hoboken and surrounding area",
    "lat": "40.7369205",
    "lng": "-74.0302510",
    "address": "56 Newark St.",
    "city": "Hoboken",
    "state": "NJ",
    "zip": "07030"
   }
}
```
