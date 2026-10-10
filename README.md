Setup: Please create a new private Github repository based on https://github.com/sardine-ai/cypress-testing-template

**Max time: 50min**

**Test**: We want you to implement the following Cypress test with JavaScript or Typescript to validate that we are correctly blocking transactions for non-supported regions in our onramp platform 

As part of your technical test, please create a simple automated test scenario featuring any framework you like and focusing on coding best practices.

Feel free to leave some comments explaining your technical decisions.


**Environment**: https://crypto.sandbox.sardine.ai
**Asset**: ETH
**Network**: ethereum
**Fiat** **currency**: USD
**OTP country**: US

**Test data
**Amount: any value
Country code: +1 (United States)
Phone: 993 472 8375
2FA: 728375 (last 6 digits of the phone number)

**Steps**
1. Open the crypto on-ramp buy page for ETH on ethereum, with fiat currency USD and OTP country US.
2. On the buy screen, enter any amount in the fiat amount field.
3. Wait until Continue is enabled, then select it.
4. Enter the phone number 9934728375. Country code +1 is already set.
5. Select the button to continue.
6. Confirm the Verify Phone Number screen is shown.
7. Enter the 2FA code 728375.
8. Confirm that "Service unavailable in your region" is displayed.

**Expected result**
After the code is accepted, "Service unavailable in your region" is visible.


**Scenario 2**

1. Proceed to create a support ticket with any content
2. Validate that the ticket was successfully created
3. Extra steps
    1. Validate that the *support* request returns successfully **{ success: true }**

Once you finish the above, please share the repo with  [sardine-interview-admin](https://github.com/sardine-interview-admin) and email your recruiter.
