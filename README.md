**Requirements: **
* OsCommerce v4
* PHP Versions >= 7.0.0 GitHub
_Note: this module has been tested only with OsCommerce v4+._


# [Plugin Handle Flow](https://github.com/annihilatoratm/drupal-doc/blob/main/README.md#plugin-handle-flow-1)

  ## Plugin İnstall

  1. Dowbnload plugin-oscommerce.zip from GitHub repository.
  2. Go to App Shop (1) -> Local storage (2) -> Upload plugin-oscommerce.zip (3).
  3. Click + sign in Action column to Install module from there.

  <img src="/images/oscommerce-1-4.png" width=60% height=60%>

  ## Plugin installation (Manual)

  1. Unpack zip.
  2. Navigate project folder lib\common\modules\orderPayment and upload unpack contents from plugin-oscommerce there.
  3. Move file ot_payneteasy.php from lib\common\modules\orderPayment to lib\common\modules\orderTotal if installer doesn't move.
  4. Move file StoredCards.php from lib\common\modules\orderPayment to lib\frontend\design\boxes\account if installer doesn't move.
  5. Move file stored-cards.tpl from lib\common\modules\orderPayment to lib\frontend\themes\basic\boxes\account if installer doesn't move.

  ## Plugin Handle Flow
  
  1. Login inside the Admin Panel and go to Modules (1) -> Payment (2) -> Online (3)
  2. Check the Payment Module Panel **PaynetEasy** is visible in the list of installed Payment Method, apply filter Show not installed, if for In-Active module use Show inactive filter.
  3. Click to PaynetEasy Payment Method and click the button *Edit* (4) under the right side panel to expand the available settings
  4. Set Enable PaynetPos to Yes, set the correct credentials, select your prefered payment method and additional settings and click Update

  <img src="/images/oscommerce-1-1.png" width=60% height=60%>
  <img src="/images/oscommerce-1-2.png" width=60% height=60%>
  
  ## Enable SurchargeFee
  
  1. Next go to Modules (1) -> Order structure (2)
  2. Check the Module SurchargeFee is visible in the list. If not installed, install it.
  3. Click to SurchargeFee and click the button Edit under the right side panel to expand the available settings
  4. Set Display Surcharge Fee to Yes, Sort Order and click Update
  5. Drag SurchargeFee above the Total Module so that surcharge fee if enable must be calculated under grand total.

  <img src="/images/oscommerce-1-3.png" width=60% height=60%>

# [Payment Flow](https://github.com/annihilatoratm/opencart-doc/blob/main/doc-eng.md#payment-flow-1)

  ## Payment Flow

  1. Please select the needed product from the main menu.

  <img src="/images/oscommerce-1.png" width=60% height=60%>
  
  2. Once the item was selected, click on "Add to basket" button to add the product to the shop cart. Pop-up message will provide with two options: select *Continue shopping* to continue explore the shop and *Go to cart* to start the payment flow. 

  <img src="/images/oscommerce-2.png" width=60% height=60%>
  <img src="/images/oscommerce-3.png" width=60% height=60%>

  3. Once *Go to cart* was chosen, press on *Pay with card* button to continue.

  <img src="/images/oscommerce-4.png" width=60% height=60%>
  
  4. Fill all required parameters on the form, confirm that you agree with the Terms & Policies, and then press the *Confirm and pay* button to finish the payment process.

  <img src="/images/oscommerce-5.png" width=60% height=60%>
  <img src="/images/oscommerce-6.png" width=60% height=60%>
