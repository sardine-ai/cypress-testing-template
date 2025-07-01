Setup: Please create a new private Github repository based on https://github.com/sardine-ai/cypress-testing-template

**Max time: 50min**

Test: We want you to implement the following Cypress test with JavaScript or Typescript to validate that we are correctly blocking transactions for non-supported regions in our onramp platform ( https://crypto.dev.sardine.ai/buy)

1. Test inputs:
    1. amount: any value
    2. Use the following phone number: 
        1. Country code: +1 (United States)
        2. 993 472 8375
    3.  2FA will be the last 6 digits of the phone number 
2. Validate that the “**Service unavailable in your region”** is displayed
3. Extra steps
    1. validate that **purchase_limit_and_risk_tags** network request shows **tag = RestrictedLocation** in the endpoint response

Scenario 2

1. Proceed to create a support ticket with any content
2. Validate that the ticket was successfully created
3. Extra steps
    1. Validate that the *support* request returns successfully **{ success: true }**

Once you finish the above, please share the repo with  [sardine-interview-admin](https://github.com/sardine-interview-admin) and email your recruiter.
