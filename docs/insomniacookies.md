## Insomnia Cookies endpoints
[insomniacookies.com](https://insomniacookies.com)

Get real-time driver location, order statuses.

## Real-time driver location
`GET https://insomniacookies.com/tracker/getDriverLocation/{order_id}`

## Status values
* `status` = `d` : `'delivered'`
* `status` = `n`   : `'not delivered'`
* `status` = `s`   : `'stopped'`
* `status` = `a` : `'up next'`

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

## Status values
* `status` = `0-3` : `'baking'`
* `status` = `4`   : `'out for delivery'`
* `status` = `5-6`   : `'delivered'`
* `status` = `99` : `'cancelled'`

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
