# API-Documentation
API Documentation

# 1. Create Order API for Single Orders

# Create Order API is used to create a gift card order & return the redemption code.
# The following are key Input elements for generating an Order.
# - Product Info
  - name : name of product from our catalog
  - code : product code from our catalog
  - quantity 1
# - Payment Info: 
  - Amount 
  - Currency 
  - method : GooglePay / ApplePay 
  - Stripe Token for fulfilling Payments made using Apple/Google Pay
  - StoreCredit amount, incase a StoreCash account credit is used to place order.
# - Sender Info
  - Sender name
  - sender Id
# - Receiver Info
  - Receiver name
  - Receiver email
      and/or
  - Phone 
# - Billing address
  - city
  - state
  - street
  - country (iso)
  - unit
  - zipcode
# - Note

# Response:
  - success or error code

Redemption URL will be sent to Receiver email id or phone number.

Create Order data will be secured in transit. Details will be shared with partners as part of integrations.

# 2. Create Order for Enterprises
  - Order creation for multiple employees is supported using an admin login from the enterprise rep. 
  - New enterprise accounts will need to be confirmed before orders can be approved.
  - Once account is approved, each of the recipients will receive redemption emails or sms messages for phone#.

