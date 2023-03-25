# API Routes
ALL routes require Authentication with the ?auth query param
## Payment
### /{version}/payment/initiate
Initiates a stripe payment
### /{version}/payment/success
Is redirected to after payment, activates record, & redirects to UI
### /{version}/payment/failed
Is redirected to after a payment fails, deactivates record, & sends email

## Orchestration
### /{version}/orchestration/createBot/:data
Creates and inits a bot on the host engine
### /{version}/orchestration/updateBot/:id/:data
Update bot data on host engine and reload it 
### /{version}/orchestration/shutdownBot/:id
Shutsdown the bot data on host engine, and disables bot
