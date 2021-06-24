# Product Added to Cart

### 

## Javascript Code
```js
window.appEventDataSAUUID = window.appEventDataSAUUID || [];
appEventDataSAUUID.push({
  "event": "Product Added to Cart",
    "cart": {
        "additionContext": "<additionContext>",
        "cartID": "<cartID>"
    },
    "eventDetails": {
        "multiAdditionDetail": "<multiAdditionDetail>",
        "multiAdditions": "<multiAdditions>"
    },
    "product": [
        {
            "productInfo": {
                "brand": "<brand>",
                "productID": "<productID>"
            }
        }
    ]
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|additionContext|string|Conveys the context of a cart addition. |PLP, PDP, Wishlist, Registry|||||||
|brand|string|Describes the brand of a product or offering.|Ford, Chevrolet, Dodge, Levis, Columbia, Patagonia|||||||
|cartID|string|Back-end identifier for a shopping cart|12345, 435678, 34567, XCV456, XCV876|||||||
|multiAdditionDetail|string|Provides details of multiple product additions to carts, wishlists, registries, etc.|all items, 3 of 5, 2 of 4|||||||
|multiAdditions|boolean|Flag indicating whether multilple products where added to carts, wishlists, registries, etc.|true, false|||||||
|productID|string|Unique Identifier of a product or offering.  Must match the format of back-end systems if used as a key for import of product meta data. Most often, one level above SKU for products with SKU variants. |155, 65588, 987764448|||||||
