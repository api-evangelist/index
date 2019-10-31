swagger: "2.0"
x-collection-name: PayPal
x-complete: 1
info:
  title: PayPal (Sandbox)
  description: bring-payments-to-apps-mobile-and-social-with-adaptive-payments-bsandbox-api-b
  version: 1.0.0
host: svcs.sandbox.paypal.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Permissions/GetAdvancedPersonalData:
    post:
      summary: Get Advanced Personal Data
      description: Use the GetAdvancedPersonalData API operation to obtain sensitive
        personal data for an account holder.
      operationId: Permissions.GetAdvancedPersonalData.post
      x-api-path-slug: permissionsgetadvancedpersonaldata-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Profiles
  /Permissions/GetBasicPersonalData:
    post:
      summary: Get Basic Personal Data
      description: Use the GetBasicPersonalData API operation to obtain basic personal
        data for an account holder.
      operationId: Permissions.GetBasicPersonalData.post
      x-api-path-slug: permissionsgetbasicpersonaldata-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Profiles
  /Permissions/CancelPermissions:
    post:
      summary: Cancel Permissions
      description: Use the CancelPermissions API operation to cancel access to a set
        of permissions.
      operationId: Permissions.CancelPermissions.post
      x-api-path-slug: permissionscancelpermissions-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Permissions
  /Permissions/GetPermissions:
    post:
      summary: Get Permissions
      description: Use the GetPermissons API operation to obtain the permissions associated
        with an access token.
      operationId: Permissions.GetPermissions.post
      x-api-path-slug: permissionsgetpermissions-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Permissions
  /Permissions/GetAccessToken:
    post:
      summary: GetAccess Token
      description: Use the GetAccessToken API operation to obtain an access token
        for a set of permissions.
      operationId: Permissions.GetAccessToken.post
      x-api-path-slug: permissionsgetaccesstoken-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Access Tokens
  /Permissions/RequestPermissions:
    post:
      summary: Request Permissions
      description: Use the RequestPermissions API operation to request permissions
        to execute API operations on a PayPal account holder???s behalf.
      operationId: Permissions.RequestPermissions.post
      x-api-path-slug: permissionsrequestpermissions-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Permissions
  /Invoice/SearchInvoices:
    post:
      summary: Search Invoices
      description: Use the SearchInvoice API operation to search an invoice.
      operationId: Invoice.SearchInvoices.post
      x-api-path-slug: invoicesearchinvoices-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Invoices
      - Search
  /Invoice/MarkInvoiceAsPaid:
    post:
      summary: Mark Invoice As Paid
      description: Use the MarkInvoiceAsPaid API operation to mark an invoice as paid.
      operationId: Invoice.MarkInvoiceAsPaid.post
      x-api-path-slug: invoicemarkinvoiceaspaid-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Invoices
  /Invoice/Cancel Invoice:
    post:
      summary: Cancel Invoice
      description: Use the CancelInvoice API operation to cancel an invoice.
      operationId: Invoice.CancelInvoice.post
      x-api-path-slug: invoicecancel-invoice-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Invoices
  /Invoice/GetInvoiceDetails:
    post:
      summary: Get Invoice Details
      description: Use the GetInvoiceDetails API operation to get detailed information
        about an invoice.
      operationId: Invoice.GetInvoiceDetails.post
      x-api-path-slug: invoicegetinvoicedetails-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Invoices
  /Invoice/UpdateInvoice:
    post:
      summary: Update Invoice
      description: Use the UpdateInvoice API operation to update an invoice.
      operationId: Invoice.UpdateInvoice.post
      x-api-path-slug: invoiceupdateinvoice-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Invoices
  /Invoice/CreateAndSendInvoice:
    post:
      summary: Create And Send Invoice
      description: Use the CreateAndSendInvoice API operation to create and send an
        invoice.
      operationId: Invoice.CreateAndSendInvoice.post
      x-api-path-slug: invoicecreateandsendinvoice-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Invoices
  /Invoice/SendInvoice:
    post:
      summary: Send Invoice
      description: Use the SendInvoice API operation to send an invoice to a payer,
        and notify the payer of the pending invoice.
      operationId: Invoice.SendInvoice.post
      x-api-path-slug: invoicesendinvoice-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Invoices
  /Invoice/CreateInvoice:
    post:
      summary: Create Invoice
      description: Use the CreateInvoice API operation to create a new invoice. The
        call includes merchant, payer, and API caller information, in addition to
        invoice detail. The response to the call contains an invoice ID and URL.
      operationId: Invoice.CreateInvoice.post
      x-api-path-slug: invoicecreateinvoice-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Invoices
  /AdaptiveAccounts/GetUserAgreement:
    post:
      summary: Get User Agreement
      description: The GetUserAgreement API operation lets you retrieve the user agreement
        for the customer to approve the new PayPal account.
      operationId: AdaptiveAccounts.GetUserAgreement.post
      x-api-path-slug: adaptiveaccountsgetuseragreement-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Aggreements
  /AdaptiveAccounts/GetVerifiedStatus:
    post:
      summary: Get Verified Status
      description: The GetVerifiedStatus API operation lets you check if a PayPal
        account status is verified. A PayPal account gains verified status under a
        variety of circumstances, such as when an account is linked to a verified
        funding source. Verified status serves to indicate a trust relationship. For
        more information about account verified status, refer to PayPal.com.
      operationId: AdaptiveAccounts.GetVerifiedStatus.post
      x-api-path-slug: adaptiveaccountsgetverifiedstatus-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Verified
      - Status
  /AdaptiveAccounts/SetFundingSourceConfirmed:
    post:
      summary: Set Funding Source Confirmed
      description: The SetFundingSourceConfirmed API operation lets your application
        set up bank accounts as funding sources for PayPal accounts.
      operationId: AdaptiveAccounts.SetFundingSourceConfirmed.post
      x-api-path-slug: adaptiveaccountssetfundingsourceconfirmed-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Verified
      - Status
  /AdaptiveAccounts/AddPaymentCard:
    post:
      summary: Add Payment Card
      description: The AddPaymentCard API operation lets your application set up credit
        cards as funding sources for PayPal accounts.
      operationId: AdaptiveAccounts.AddPaymentCard.post
      x-api-path-slug: adaptiveaccountsaddpaymentcard-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Credit Card
  /AdaptiveAccounts/AddBankAccount:
    post:
      summary: Add Bank Account
      description: The AddBankAccount API operation lets your application set up bank
        accounts as funding sources for PayPal accounts.
      operationId: AdaptiveAccounts.AddBankAccount.post
      x-api-path-slug: adaptiveaccountsaddbankaccount-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Bank Account
  /AdaptiveAccounts/CreateAccount:
    post:
      summary: Create Account
      description: The CreateAccount API operation enables you to create a PayPal
        account on behalf of a third party.
      operationId: AdaptiveAccounts.CreateAccount.post
      x-api-path-slug: adaptiveaccountscreateaccount-post
      parameters:
      - in: header
        name: X-PAYPAL-SANDBOX-EMAIL-ADDRESS
      responses:
        200:
          description: OK
      tags:
      - Payments
  /AdaptivePayments/GetFundingPlans:
    post:
      summary: Get Funding Plans
      description: Use the GetFundingPlans API operation to determine the funding
        sources that are available for a specified payment, identified by its key,
        which takes into account the preferences and country of the receiver as well
        as the payment amount. You must be both the sender of the payment and the
        caller of this API operation
      operationId: AdaptivePayments.GetFundingPlans.post
      x-api-path-slug: adaptivepaymentsgetfundingplans-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Plans
  /AdaptivePayments/GetShippingAddresses:
    post:
      summary: Get Shipping Addresses
      description: Use the GetShippingAddresses API operation to obtain the selected
        shipping address. You must have created the payment or preapproval key that
        identifies the account holder whose shipping address you want to obtain, or
        be the primary receiver of the payment or one of the parallel receivers of
        the payment. The shipping address is available only if it was provided during
        the embedded payment flow.
      operationId: AdaptivePayments.GetShippingAddresses.post
      x-api-path-slug: adaptivepaymentsgetshippingaddresses-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Addresses
  /AdaptivePayments/ExecutePayment:
    post:
      summary: Execute Payment
      description: The ExecutePayment API operation lets you execute a payment set
        up with the Pay API operation with the actionType CREATE. To pay receivers
        identified in the Pay call, set the pay key from the PayResponse message in
        the ExecutePaymentRequest message.
      operationId: AdaptivePayments.ExecutePayment.post
      x-api-path-slug: adaptivepaymentsexecutepayment-post
      responses:
        200:
          description: OK
      tags:
      - Payments
  /AdaptivePayments/SetPaymentOptions:
    post:
      summary: Set Payment Options
      description: "You use the SetPaymentOptions API operation to specify settings
        for a payment of the actionType CREATE. \n\t\t\t\t\tThis actionType is specified
        in the PayRequest message."
      operationId: AdaptivePayments.SetPaymentOptions.post
      x-api-path-slug: adaptivepaymentssetpaymentoptions-post
      responses:
        200:
          description: OK
      tags:
      - Payments
  /AdaptivePayments/GetPaymentOptions:
    post:
      summary: Get Payment Options
      description: You use the GetPaymentOptions API operation to retrieve the payment
        options passed with the SetPaymentOptionsRequest.
      operationId: AdaptivePayments.GetPaymentOptions.post
      x-api-path-slug: adaptivepaymentsgetpaymentoptions-post
      responses:
        200:
          description: OK
      tags:
      - Payments
  /AdaptivePayments/Refund:
    post:
      summary: Refund
      description: Use the Refund API operation to refund all or part of a payment.
        You can specify the amount of the refund and identify the accounts to receive
        the refund by the payment key or tracking ID, and optionally, by transaction
        ID or the receivers of the original payment.
      operationId: AdaptivePayments.Refund.post
      x-api-path-slug: adaptivepaymentsrefund-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Refunds
  /AdaptivePayments/ConvertCurrency:
    post:
      summary: Convert Currency
      description: Use the ConvertCurrency API operation to request the current foreign
        exchange (FX) rate for a specific amount and currency.
      operationId: AdaptivePayments.ConvertCurrency.post
      x-api-path-slug: adaptivepaymentsconvertcurrency-post
      responses:
        200:
          description: OK
      tags:
      - Payments
      - Currency
  /AdaptivePayments/CancelPreapproval:
    post:
      summary: Cancel Preapproval
      description: Use the CancelPreapproval API operation to handle the canceling
        of preapprovals. Preapprovals can be canceled regardless of the state they
        are in, such as active, expired, deactivated, and previously canceled.
      operationId: AdaptivePayments.CancelPreapproval.post
      x-api-path-slug: adaptivepaymentscancelpreapproval-post
      responses:
        200:
          description: OK
      tags:
      - Payments
  /AdaptivePayments/PreapprovalDetails:
    post:
      summary: Preapproval Details
      description: Use the PreapprovalDetails API operation to obtain information
        about an agreement between you and a sender for making payments on the sender???s
        behalf.
      operationId: AdaptivePayments.PreapprovalDetails.post
      x-api-path-slug: adaptivepaymentspreapprovaldetails-post
      responses:
        200:
          description: OK
      tags:
      - Payments
  /AdaptivePayments/Preapproval:
    post:
      summary: Preapproval
      description: 'Use the Preapproval API operation to set up an agreement between
        yourself and a sender for making payments on the sender???s behalf. You set
        up a preapprovals for a specific maximum amount over a specific period of
        time and, optionally, by any of the following constraints: the number of payments,
        a maximum per-payment amount, a specific day of the week or the month, and
        whether or not a PIN is required for each payment request.'
      operationId: AdaptivePayments.Preapproval.post
      x-api-path-slug: adaptivepaymentspreapproval-post
      responses:
        200:
          description: OK
      tags:
      - Payments
  /AdaptivePayments/PaymentDetails:
    post:
      summary: Payment Details
      description: Use the PaymentDetails API operation to obtain information about
        a payment. You can identify the payment by your tracking ID, the PayPal transaction
        ID in an IPN message, or the pay key associated with the payment.
      operationId: AdaptivePayments.PaymentDetails.post
      x-api-path-slug: adaptivepaymentspaymentdetails-post
      responses:
        200:
          description: OK
      tags:
      - Payments
  /AdaptivePayments/Pay:
    post:
      summary: Pay
      description: Use the Pay API operation to transfer funds from a sender???s PayPal
        account to one or more receivers??? PayPal accounts. You can use the Pay API
        operation to make simple payments, chained payments, or parallel payments;
        these payments can be explicitly approved, preapproved, or implicitly approved.
      operationId: AdaptivePayments.Pay.post
      x-api-path-slug: adaptivepaymentspay-post
      responses:
        200:
          description: OK
      tags:
      - Payments