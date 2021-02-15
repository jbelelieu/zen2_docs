# GENERAL RULES

- When unsure about something, esp something security related, give people control via an option, but make the default the more secure option.

- 

# Known Bugs

- CartReceipt Email subject: Order #%transactionId% complete
- Add premium_membership into cart: {"data":{"details":null,"code":"E034","message":"You can only have %max% of this product per cart"}}
    - Notice the "%max%"
- DELETE/GET for services isn't saving the details in the logs.
    - Need to see why that isn't working...
- I can't update ID for an invoice...
    - DTO setId is called when controller passed DTO to service.

# TODO

- Given that we've added tabs to the FE, we can assume that the LIST / GET methods don't need everything that the
  getEntity() returns by default. We need a setting to say "JUST THIS PRIMARY ENTITY".

- Licenses/dig files: current version for "am I up to date".
    - Maybe licensing is going too far eh... is this a licenseing platform?

- Make sure when an invoice payment is made, if it is a partial payment, it will not make future payments forbidden (status of the cart).

- Heavy caching on various GET / LIST endpoints.

- *** Search for all TODO in codebase: and complete them!

- Test Signup again since trait was added.
- Test logout.

- TODO: UPDATE resource controllers (product, invoice, user)

- Get CRON JOBS up and running

- Route all emails through a class that determines the user's desired contact settings??

- Login using Apple & Google

- Post order need to log in metadata the address it was billed/shipped to in case that address gets deleted.

- GDPR Compliance
    - Deletion of data
    - Acceptance of cookies

- Captcha on forms

- Coding practices:
    - declare services in constructor
    - function ordering standards
    - better comments
        - @bodyParam on all controller comments
    - Go back to earliest classes you wrote (date created) and make sure they're inline with newer coding standards

- Move error codes to DB to allow for updating from the admin.

- On Delete:
    - Allow for input of a "reason".

- Online guest session grants.

- Address Management
    - Add new address on file
    - Delete Address on File **DONE**

- Criteria System:
    - Ability to run two or more reports and then cross reference the results.
    - Allow things like "within the last x days/weeks/etc."

Login Types
- Auth app integration
- No password login.
- In-person: Simple QR scanning pass system
- Guest Session/Pass
    - Sample Flow:
        - Grant type = SESSION
        - Check user_grant.seats to see how many they can offer against how many have been granted/used.
    - What about recurring???

Caching System On Requests
- DB-driver + Redis-driver

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

Squeeze Pages?

- Export Data
- Import Data

- Page Statistics?
    - Products Viewed
      ( might wanna leave this shit to google )

Source tracking on registration, etc..
    - When each request comes in, if the "sti" cookie is present, track that.

WordPress Integration?

Email Autoresponders + Campaigns
    - Criteria based

Cron Jobs
    - See folder
    - Password change force (based on option)

Integrations
- Intercom
- Freshdesk
- Zendesk

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

# FUTURE VERSIONS

- Events + Event Management
- Public member search + directory
    - Avatars (use google, apple, or gravitar ones if possible)

# Unsure

- Require additional payment when redeeming a guest pass?
    - Unlikely to have big benefit?
- Affiliate program?

# BLOCKED

-

# DONE

- Translate (localize) email subjects + templates.
- Update email
    - Requires confirmation via code before completing the update.
- Update user information (UserController::updateUserData)
    - Determine fields that can be updated.
    - Validate against those fields.
- COPYRIGHT AT THE TOP OF EVERY FILE!!!!

