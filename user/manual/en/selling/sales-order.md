<!-- add-breadcrumbs -->
# Sales Order

The Sales Order confirms the receipt of an order from your customer. It is usually a binding Contract with your Customer. Once your customer confirms the Quotation you can convert your Quotation into
a Sales Order.

There are various transactions which can be triggered from Sales Order like;

* Delivery Note
* Sales Invoice
* Material Request
* Production Order
* Project

<img class="screenshot" alt="Sales Order flow" src="{{docs_base_url}}/assets/img/selling/sales-order-f.jpg">

### 1. How to create a Sales Order
1. Go to **Selling > Sales > Sales Order > New Sales Order** or Type 'New Sales Order' into the "Global Search" field.

   1. Enter Customer name.
   1. Under "Delivery Date" set the date by which order is to be delivered.
   1. With Order Type you can set whether it's a Sales order, Maintenance order, or from the online [Shopping Cart](/docs/user/manual/en/website/shopping-cart) of your website. By default this value is set to "Sales"
   1. In the "Customer's Purchase Order" you can enter the Customers Purchase Order No. or other details which may be useful as a reference.
   1. Under "Set Source Warehouse", you define the warehouse from which the item will be ordered. If the Items in that Sales Order do **not** have checked the "Maintain Stock" Box this can be left blank.
   1. Enter the items and quantities to be delivered in the Item table. In case you have Setup Item Prices for the items in question the "Rate" (price per Unit) will be populated automacially. If not, put the item Rate manually. You can also overwrite the auto-populated Item Rate in case you want to change that value.
   1. Click "Save" to save a draft of the Sales Order and    
   1. "Submit" to submit the Sales Order to the System.


2. You can also create a Sales Order from a submitted Quotation.

    <img class="screenshot" alt="Make Sales Order from Quotation" src="{{docs_base_url}}/assets/img/selling/make-SO-from-quote.png">

3. Or you can create a new Sales Order and pull details from a Quotation.

    <img class="screenshot" alt="Make Sales Order from Quotation" src="{{docs_base_url}}/assets/img/selling/make-so.gif">

Most of the information in your Sales Order is the same as in the Quotation.

There are a few amongst other things that a Sales Order will ask you to
update.

  * Enter Delivery Date against each item. If there are multiple items and if you enter a delivery date in the first row, the date will be copied to other rows as well where it is blank.
  * Customer Purchase Order number: If your customer has sent you a Purchase Order, you can update its number for future reference (in billing).
  * To allow for per-Customer, per-Item Pricing Rules ("Customer A" pays $1.00 for "Item 1" but "Customer B" pays $1.25 for "Item 1"), there's a check box in Selling Settings to enable saving the specific item price per customer when you change a price in the Sales Order.

### 2. Features
#### 2.1 Packing List

The “Packing List” table will be automatically updated when you “Save” the Sales Order. If any Items in your table are Product Bundle (packets), then the “Packing List” will contain the exploded (detailed) list of your Items.

#### 2.2 Reservation and Warehouses

If your Sales Order contains Items for which inventory is tracked (Is Stock Item is “Yes”) then, ERPNext will ask you for “Reservation Warehouse”. If you have set a default Warehouse for the Item, it will automatically set this Warehouse here.

This “reserved” quantity will help you project what is the quantity you need to purchase based on all your commitments.

#### 2.3 Taxes

To add taxes to your Quotation, you can select a **Sales Taxes and Charges Template** or add the taxes on your own.

For example:

<img class="screenshot" alt="Taxes and Charges" src="{{docs_base_url}}/assets/img/selling/taxes-and-charges.gif">

To understand taxes in detail visit [Taxes](/docs/user/manual/en/setting-up/setting-up-taxes.html).

#### 2.4 Sales Team

**Sales Partner:** If this Sale was booked via a Sales Partner, you can update the Sales Partner’s details with commission and other info that you can aggregate.

**Sales Persons:** ERPNext allows you to tag multiple Sales Persons who may have worked on this deal. You can also split the amount in targets of different Sales Persons and track how much incentives they earned on this deal.

#### 2.5 Next Steps

Once you “Submit” your Sales Order, you can now trigger different aspects of
your organization:

  * To begin purchase click on Make -> Purchase Request
  * To make a shipment entry click on Make -> Delivery Note. You can also make Delivery Note for selected items based on delivery date.
  * To bill, make Make -> Sales Invoice
  * To stop further process on this Sales Order, click on “Stop”

#### 2.6 Submission

Sales Order is a “Submittable” transaction. See Document Stages. You will be able to execute dependent steps (like making a Delivery Note) only after “Submitting” this Sales Order.

#### 2.7 Sales Order with Order type Maintenance

When the 'Order Type' of the Sales Order is 'Maintenance' follow the steps
given below:

1. Enter Currency, Price list and Item details.

2. Mention taxes and other information.

3. Save and Submit the form

4. Once the form is submitted, the Action button will provide three choices.

    i) Maintenance Visit ii) Maintenance Schedule iii) Invoice.


> **Note 1:**   
By clicking on the Action button and selecting 'Maintenance Visit' you can directly fill the visit form. The Sales Order details will be fetched directly.    

> **Note 2:**    
By clicking on the Action button and selecting 'Maintenance Schedule' you can fill the schedule details. The Sales Order details will be fetched directly.

> **Note 3:**    
By clicking on the Invoice button you can make an Invoice for your
services . The sales orders details will be fetched directly.

#### 3. Related Topics
1. [Quotation](/docs/user/manual/en/selling/quotation)
1. [Close Sales Order](/docs/user/manual/en/selling/articles/close-sales-order)
1. [Amending Sales Order After Submit](/docs/user/manual/en/selling/articles/amending-sales-order-after-submit)
