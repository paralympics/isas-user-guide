# Licence Packages for NFs

For individual sports, NFs acquire licences in packages and then issue them to their athletes. This section lists all registered packages that the
user can access, past and current, with most information about the package directly available from the result matrix. Users can restrict the list by
NF season, sport and invoice number.

| Field              | Format                                         | Comments                                                                              |
|--------------------|------------------------------------------------|---------------------------------------------------------------------------------------|
| Licence Package    | Code                                           | allocated on package purchase, same as invoice number                                 |
| NF                 | Read-only text field                           | drop down box on package purchase form                                                |
| Season             | Read-only text field                           | drop down box on package purchase form                                                |
| Sport              | Read-only text field                           | drop down box on package purchase form; default is to make available to all sports    |
| Status             | Read-only text field                           | confirmed on payment reception                                                        |
| Invoice Recipient  | Read-only text area [specified on application] | not viewable from result matrix                                                       |
| Package Price      | Read-only integer                              | package price in EUR without VAT                                                      | 
| Package Name       | Read-only text field                           |
| Available Licences | Read-only integer                              | current count of available remaining licences under this package.                     |
| Total Licences     | Read-only integer                              | all licences in the package                                                           |
| NF Comments        | text area                                      | editable from the detail page for any comments from NF side regarding the application |

NFs acquire packages through clicking the _Add License Package_ button, either from the search form or from the details screen. This form, shown in
Figure 5.1, is specifically designed to only provide the relevant options for a purchase, and to illustrate possible savings by buying in bulk.

A buyer then enters their specific data in the fields, as described in the table below, before clicking _Submit Order_ to complete the purchase.

| Field                                                                               | Format                  | Comments                                                                                                       |
|-------------------------------------------------------------------------------------|-------------------------|----------------------------------------------------------------------------------------------------------------|
| NF                                                                                  | Drop-down box [NF]      | restricted by permission – usually only one choice for any user, e.g. NF Japan can only select Japan           |
| Season                                                                              | Drop-down box [season]  | only seasons with Active status are selectable                                                                 | 
| Sport                                                                               | Drop-down box [sport]   |                                                                                                                |
| License Package                                                                     | Radio boxes, choose one | all Active packages are listed with name, number of licenses, price in EUR and comments                        | 
| Payment Method                                                                      | Radio box, choose one   | currently, only bank transfer is offered; please contact IBSA for other arrangements                           |
| <span class="table-header">Invoice Recipient </span><span class="asterisk">*</span> |                         |                                                                                                                |
| Address of Recipient                                                                | Drop-down box           | The address of a previously saved recipient can be loaded from here. This will disable the other input fields. |
| Organisation                                                                        | Text field              | Postal name                                                                                                    |
| Street / P.O Box                                                                    | Text field              | Address                                                                                                        | 
| Postal Code & City                                                                  | Text field              |                                                                                                                |
| Country                                                                             | Text field              | Name in English                                                                                                |
| Save in address box                                                                 | Checkbox                | Tick to save for use later ([Address Book](licence-management/address-book))                                   | 

<p class="footnote">
    <small><span class="asterisk">*</span>If empty, the NF default address - currently consisting of the official NF name only - is printed on the invoice PDF as recipient. Otherwise, the address specified here is used in the invoice's header.</small>
</p>

Once the order is submitted, the user processes the invoice and bank payments, and then waits for IBSA to confirm the payment using the Invoices
screen of ISAS. This is described in more details in [Invoices](licence-management/invoices). The package is listed as **Pending** from the search
form until this confirmation is obtained, and the package can not be used to license further athletes until payment is confirmed and the status is
changed to **Paid**.

<figure>
    <img src="_img/figures/5.1-license-package-form.png" alt="Buy NF License Package form" class="screenshot" >
    <figcaption>Figure 5.1 - Buy NF License Package form</figcaption>
</figure>