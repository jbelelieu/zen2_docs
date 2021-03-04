# TODO

## other

- *** Search for all TODO in codebase: and complete them!

- Terms and Conditions
    - Signed agreements stored in db
        - Blockchain tie in here hashed onchain?
        (
            Or maybe not because the idea is the frontend renders terms?
            This doesn't work for non-technical people who want a GUI interface to create this shit in.
        )
        - Terms should be associated a grant!
            - When you're about to register or buy something, we determine all the terms you have
              to agree to and then send them back, requiring Proof-Of-Signature via a hash of the
              SALT + USER NAME + TERM HASH

Payment Gateways
- PayPal Integration
    - https://developer.paypal.com/docs/connect-with-paypal/integrate/
- Authorize.Net
    - 
- 2CheckOut
    - 
- Square
    - 
- Braintree 
    -
- WePay
    - 
- Worldpay (int)
- Alipay (asia)
- Apple Pay Integration
    - https://developer.apple.com/documentation/apple_pay_on_the_web/
- Venmo Integration?
    - 

# CODE QUALITY

- Bind interfaces to container
    - https://laravel.com/docs/8.x/container#binding-interfaces-to-implementations
- DTOs: trim and clean up all incoming data (normalize);
- For all DELETE/UPDATE, make sure the user updating is the user who created it.
