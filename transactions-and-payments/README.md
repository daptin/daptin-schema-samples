# Payment data model moved

The old standalone `sale` and `payment` schema existed only to support the
retired PayPal example. The maintained checkout example now composes
`api_plan`, `api_member`, provider integration actions, and owned checkout
records instead:

- [Payment checkout example](https://github.com/daptin/daptin/tree/master/examples/payment-checkout)
- [Payments and Checkout guide](https://github.com/daptin/daptin/wiki/Payments-and-Checkout)
