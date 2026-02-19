# User Story

## User Story
As a registered user  
I need to be able to reset my password  
So that I can regain access to my account if I forget it

## Acceptance Criteria

Scenario 1: Successful password reset
Given a registered user is on the login page
When the user clicks "Forgot Password" and enters their registered email
Then the user receives a password reset email

Scenario 2: Unregistered email attempt
Given a user is on the login page
When the user clicks "Forgot Password" and enters an unregistered email
Then the user sees an error message saying "Email not found"

Scenario 3: Reset link expires
Given a user has requested a password reset
When 24 hours have passed since the reset email was sent
Then the password reset link becomes invalid and the user is prompted to request a new link
