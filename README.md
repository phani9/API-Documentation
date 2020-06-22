# API-Documentation

## 1. Create Order API for Single Orders
Create Order API is used to create a gift card order & return the redemption code.

### Request (Key elements):
- ##### Product Info
    - Name: Product Name from our catalog
    - Code: Product Code from our catalog
    - Quantity: 1
- ##### Payment Info
    - Amount
    - Currency
    - Method: GooglePay / ApplePay
    - Stripe Token for fulfilling Payments made using Apple/Google Pay
    - StoreCredit amount, incase a StoreCash account credit is used to place order.
- ##### Sender Info
    - Sender Name
    - Sender ID
- ##### Receiver Info
    - Receiver Name
    - Receiver Email and/or
    - Receiver Phone
- ##### Billing Address
    - City
    - State
    - Street
    - Country (ISO Code)
    - Unit
    - Zip-Code
- ##### Note (String)

### Response:
- ##### HTTP Status Code
- ##### Message (String)

Redemption URL will be sent to Receiver email id or phone number.

Create Order data will be secured in transit. Details will be shared with partners as part of integrations.

## 2. Create Order for Enterprises
  - Order creation for multiple employees is supported using an admin login from the enterprise representative in portal. 
  - New enterprise accounts will need to be confirmed before orders can be approved.
  - Once account is approved, each of the recipients will receive redemption emails or sms messages for phone#.

