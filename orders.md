Orders
=====

# Create order
`POST /orders.json` Create new pik

### Request Data

```
{
	"order": {
		"recipient_phone":"{{recipient_phone_number}}",
		"recipient_name":"{{recipient_name}}",
		"total":"{{order_price}}",
		"uuid":"{{order_id}}" 
	}
}

```


### Response Data
The response is given in JSON format

```
{
    "order": {
        "id": 1,
        "shop_id": "1",
        "recipient_phone": "",
        "recipient_name": "{{recipient_name}}",
        "total": "{{order_price}}",
        "uuid": "{{order_id}}",
        "created_at": "2020-12-13T16:24:01.364Z",
        "updated_at": "2020-12-13T16:24:01.364Z",
        "status": 0
    },
    "pik": {
        "id": 1,
        "order_id": 1,
        "slot": null,
        "vehicle": null,
        "starttime": null,
        "endtime": null,
        "date": "2020-12-13",
        "status": "pending",
        "checkin": null,
        "piked": null,
        "created_at": "2020-12-13T16:24:01.369Z",
        "updated_at": "2020-12-13T16:24:01.369Z",
        "uuid": "{{pik_uuid}}",
    }
}
```
