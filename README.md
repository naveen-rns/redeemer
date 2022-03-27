# CASHBACK | LOYALTY | VOUCHERS | PAYMENTS

Method of transaction

1. Payment through online store

  a. Payment through Crypto Bridge. Paying via crypto

  b. Payment through Credit Card / Paynow / Paypal

2. Payment in physical store

  a. Payment with Cash

1.a - Payment through Crypto Bridge

In this methhod the cusomer is paying through crypto. So one atomic transaction can be created for two underlying transactions. 
TXN #1 - Payment via crypto from customer to merchant
TXN #2 - Transfer of loyalty points from merchant to customer

The proof of payment is on-chain so it is easy to implement the atomic transaction.
1.b - Payment through Credit Card / Paynow / Paypal

In this methhod the cusomer is paying through traditional methods
TXN #1 - Payment from customer to merchant via Credit Card / Paynow / Paypal
TXN #2 - Transfer of loyalty points from merchant to customer

In this case For the proof of payment, the on-chain program has to rely on the offchain transaction id that is secured by the TLS (Transport Layer Security) communication.
TXN #2 happens only after TXN #1 is confirmed.
For TXN #2
  i. The system will generate a QR Code to the customer
  ii. On the QR code if the customer does not have connected wallet then torus wallet window is displayed to user with enter social logins
  iii. Then the loyalty points are transferred to this connected wallet.
        Exploring two ways to make this happen
        1. System auto transfers to this wallet - Gas is paid by the system.
        2. Customer pulls the points from the system to his wallet. Gas is paid by the user.
2.a - Payment with Cash

  TXN #1 - Payment from customer to merchant via Cash in store. Store manager giving receipt to customer with QR Code printed.
  TXN #2 - Customer scans the QR Code on receipt and loyalty points transferred from merchant to customer. 
  This flow will be same as 1.b TXN2.
