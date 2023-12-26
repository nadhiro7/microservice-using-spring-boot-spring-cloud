API-GateWay
-----------
```bash
URL : http://localhost:8989/order/bookOrder
HTTP Method : POST
```
Json Request :
```json
{
  "order": {
    "name": "phone",
    "id": 1,
    "price": 999,
    "qte": 1
  },
  "payment": {

  }
}
```
Json Response :
```json
{
  "order": {
    "id": 1,
    "name": "phone",
    "qte": 1,
    "price": 999.0
  },
  "amount": 999.0,
  "transactionId": "30f03fb9-2d7c-4bf9-b6c6-6b9fe0568fe9",
  "message": "payment processing successful and order placed"
}

```
```bash
URL : http://localhost:8989/payment/1
HTTP Method : GET
```
Json Response :
```json
{
    "paymentId": 1,
    "transactionId": "30f03fb9-2d7c-4bf9-b6c6-6b9fe0568fe9",
    "orderId": 1,
    "paymentStatus": "SUCCESS",
    "amount":999
}
```
