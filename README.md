# Pay pal
Paypal checkout  application allows for online  payment and card payments optional transactions using the paypal api from the paypal payment platform

<h5>Reqiurements<h5> 

const mongoose = require('mongoose');

require('dotenv').config();

require("dotenv").config()

const port = process.env.PORT || 5000;
 
const paypal = require("@paypal/checkout-server-sdk")

<h5>Note<h5> 
<p>Currency is always in USD CENTS  <p>


<h5>APPP COMPONENETS INDEX:-<h5> 

1.NODE DEPENDENCIES

2.ENV

3.ROUTES/ENDPOINTS 

 
<h5>APP COMPONENETS :-<h5>

<h5>1. NODE DEPENDENCIES =========================================================================<h5>
<p>
"@paypal/checkout-server-sdk": "^1.0.3",  

"cors": "^2.8.5",

"dotenv": "^16.0.0",

"express": "^4.17.3",

"mongoose": "^6.2.3", 

"devDependencies": {
    "nodemon": "^2.0.15"
  }
</p>

<h5>
<h5>

1. Git ignore files ===============================================================================

      node_module

      .env

<h5>

2. env  ============================================================================
</h5>

      ATLAS_URI=mongodb+srv://<UserName>:<password>.4p1ws.mongodb.net/myFirstDatabase?retryWrites=true&w=majority

      PAYPAL_CLIENT_ID=<ClientID>

      PAYPAL_CLIENT_SECRET=<CLIENT SECRET>

<h5>


3. ROUTES/ENDPOINTS (index.js) ============================================================================

Routes:

</h5>
<p> 

3.1   Route:  /          (index)

      type: Get

      Response-:
            
            render(Index view)


3.2 Route:  /create-order

      type: Post

      Response-:
            
            {
                  reference_id: 'default',

                  amount: { currency_code: 'USD', value: '800.00', breakdown: [Object] },
                  
                  payee: {

                        email_address: 'sb-spfr31898020@personal.example.com',

                        merchant_id: 'D4EK62QGSMS68'

                  },

                  items: [ [Object], [Object] ]

            }

</p>




