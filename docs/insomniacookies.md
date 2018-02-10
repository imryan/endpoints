## Insomnia Cookies endpoints
[insomniacookies.com](https://insomniacookies.com)

Get real-time driver location, order statuses.

## Real-time driver location
`GET https://insomniacookies.com/tracker/getDriverLocation/{order_id}`

### Status values
* `status` = `d` : `'delivered'`
* `status` = `n`   : `'not delivered'`
* `status` = `s`   : `'stopped'`
* `status` = `a` : `'up next'`

### Response:
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

### Parameters:
- `trackingID` : `'779725445b8610e2'`

### Status values
* `status` = `0-3` : `'baking'`
* `status` = `4`   : `'out for delivery'`
* `status` = `5-6`   : `'delivered'`
* `status` = `99` : `'cancelled'`

### Response:
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

## Cart
`GET https://insomniacookies.com/shop/getCart`

### Parameters:
- `insomnia_cookie` : Some kind of cookie from the site (ha ha)

### Response:
```
{
  "store": [],
  "products": [],
  "totals": {
    "subtotal": "0.00",
    "shipping": "0.00",
    "tax": "0.00",
    "is_tax_exempt": false,
    "total_before": "0.00",
    "total": "0.00",
    "loyalty": 0,
    "loyalty_amount": "0.00",
    "coupon_amount": "0.00",
    "tip": "0.00",
    "giftcard_amount": "0.00",
    "freeProduct": "0.00"
  },
  "coupon": false,
  "shipping": false,
  "upsell": {
    "upsell": 0
  },
  "loyalty_show_signup": false,
  "loyalty_text": "You're not logged in! You could be earning  points for this order.",
  "numProducts": 0,
  "products_debug": [],
  "has_shipping": false
}
```

## Get product
`GET https://insomniacookies.com/shop/getProduct/{product_id}/{delivery|ship|pickup}`

### Parameters:
- `product_id` : ID of product (try 225)
- `delivery_option` : `delivery|ship|pickup`

### Response:
```
{
  "product": {
    "productID": "225",
    "price": "26.00",
    "title": "12 Cookie Gift Box",
    "description": "Choose one of our perfect gift solutions for clients, friends, and family! Our customized gifts allow you to choose an assortment of cookies delivered in beautiful packaging.",
    "image": "whitegiftbox_1000xtrans1.png",
    "resident": "0",
    "diff_tax": "0",
    "is_packaging": "0",
    "type": "both",
    "maximum": "0",
    "max_quantity": "0",
    "featured": "0",
    "show_image": "0",
    "oos": "0",
    "groups": "1",
    "tax_amount": "0.00",
    "category": "Ship Cookies"
  },
  "options": [
  {
  "sub": [
  {
    "productID": "4",
    "title": "Chocolate Chunk",
    "image": "choc-chunk.png",
    "diff_tax": "0",
    "is_packaging": "0",
    "optionID": "1399",
    "price": "0.00"
  },
  {
    "productID": "16",
    "title": "Double Chocolate Chunk",
    "image": "dbl-choc-chunk.png",
    "diff_tax": "0",
    "is_packaging": "0",
    "optionID": "1401",
    "price": "0.00"
  },
  {
    "productID": "14",
    "title": "Double Chocolate Mint",
    "image": "dbl-choc-mint.png",
    "diff_tax": "0",
    "is_packaging": "0",
    "optionID": "1402",
    "price": "0.00"
  },
  {
    "productID": "15",
    "title": "Classic with M&M's",
    "image": "mm.png",
    "diff_tax": "0",
    "is_packaging": "0",
    "optionID": "1403",
    "price": "0.00"
  },
  {
    "productID": "5",
    "title": "Oatmeal Raisin",
    "image": "oatmeal-raisin.png",
    "diff_tax": "0",
    "is_packaging": "0",
    "optionID": "1404",
    "price": "0.00"
  },
  {
    "productID": "12",
    "title": "Peanut Butter Chip",
    "image": "pb-chip.png",
    "diff_tax": "0",
    "is_packaging": "0",
    "optionID": "1405",
    "price": "0.00"
  },
  {
    "productID": "13",
    "title": "Snickerdoodle",
    "image": "snickerdoodle.png",
    "diff_tax": "0",
    "is_packaging": "0",
    "optionID": "1406",
    "price": "0.00"
  },
  {
    "productID": "6",
    "title": "Sugar",
    "image": "sugar.png",
    "diff_tax": "0",
    "is_packaging": "0",
    "optionID": "1407",
    "price": "0.00"
  },
  {
    "productID": "11",
    "title": "White Chocolate Macadamia",
    "image": "white-maca.png",
    "diff_tax": "0",
    "is_packaging": "0",
    "optionID": "1408",
    "price": "0.00"
  }
 ],
  "properties": {
    "title": "Cookie Flavor",
    "type": "textbox",
    "max": "0",
    "total": "12",
    "assortment": "1",
    "description": "",
    "groupID": "1"
  }
}
  ],
  "success": true,
  "view": "product"
}
```

## Login
`POST https://insomniacookies.com/user/login/json`

### Parameters:
- `email` : Your email
- `password` : Your password

### Response:
```
{
  "body": {
    "rememberMe" : null,
    "message" : "Login successful!",
    "firstname" : "Ryan"
   },
   "success":1
}
```
