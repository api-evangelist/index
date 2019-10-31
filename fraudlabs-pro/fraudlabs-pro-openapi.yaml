swagger: "2.0"
x-collection-name: FraudLabs Pro
x-complete: 1
info:
  title: FraudLabs Pro
  description: online-payment-fraud-detection-service--it-helps-merchants-to-minimize-chargebacks-and-therefore-maximize-the-revenue--it-can-be-used-to-detect-fraud-for-various-kinds-of-payment-method-such-as-credit-card-paypal-cod-and-so-on--please-visit-httpswww-fraudlabspro-com-to-learn-more-
  version: 1.0.0
host: virtserver.swaggerhub.com
basePath: /fraudlabspro/fraudlabspro/1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/order/screen:
    post:
      summary: V1OrderScreen_POST
      description: Screen order for payment fraud.
      operationId: V1OrderScreenPost
      x-api-path-slug: v1orderscreen-post
      parameters:
      - in: query
        name: amount
      - in: query
        name: avs_result
      - in: query
        name: bill_addr
      - in: query
        name: bill_city
      - in: query
        name: bill_country
      - in: query
        name: bill_state
      - in: query
        name: bill_zip_code
      - in: query
        name: bin_no
      - in: query
        name: card_hash
      - in: query
        name: currency
      - in: query
        name: cvv_result
      - in: query
        name: department
      - in: query
        name: email
      - in: query
        name: email_domain
      - in: query
        name: email_hash
      - in: query
        name: first_name
      - in: query
        name: flp_checksum
      - in: query
        name: format
      - in: query
        name: ip
      - in: query
        name: key
      - in: query
        name: last_name
      - in: query
        name: password_hash
      - in: query
        name: payment_mode
      - in: query
        name: quantity
      - in: query
        name: ship_addr
      - in: query
        name: ship_city
      - in: query
        name: ship_country
      - in: query
        name: ship_state
      - in: query
        name: ship_zip_code
      - in: query
        name: username_hash
      - in: query
        name: user_order_id
      - in: query
        name: user_order_memo
      - in: query
        name: user_phone
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Fraud
  /v1/order/feedback:
    post:
      summary: V1OrderFeedback_POST
      description: Feedback the status of an order transaction.
      operationId: V1OrderFeedbackPost
      x-api-path-slug: v1orderfeedback-post
      parameters:
      - in: query
        name: action
      - in: query
        name: format
      - in: query
        name: id
      - in: query
        name: key
      - in: query
        name: notes
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Fraud
      - Feedback