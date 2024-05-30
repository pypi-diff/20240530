# Comparing `tmp/monei-1.2.5.tar.gz` & `tmp/monei-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monei-1.2.5.tar", last modified: Mon May  6 16:31:52 2024, max compression
+gzip compressed data, was "monei-1.2.6.tar", last modified: Thu May 30 14:03:16 2024, max compression
```

## Comparing `monei-1.2.5.tar` & `monei-1.2.6.tar`

### file list

```diff
@@ -1,206 +1,206 @@
-drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2024-05-06 16:31:52.501413 monei-1.2.5/
-drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2024-05-06 16:31:52.463049 monei-1.2.5/Monei/
--rw-r--r--   0 dmitriy    (501) staff       (20)     6011 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/__init__.py
-drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2024-05-06 16:31:52.465364 monei-1.2.5/Monei/api/
--rw-r--r--   0 dmitriy    (501) staff       (20)      293 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/api/__init__.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     7936 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/api/apple_pay_domain_api.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     7513 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/api/bizum_api.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    60407 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/api/payments_api.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    40355 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/api/subscriptions_api.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    27077 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/api_client.py
-drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2024-05-06 16:31:52.465557 monei-1.2.5/Monei/apis/
--rw-r--r--   0 dmitriy    (501) staff       (20)      599 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/apis/__init__.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    14455 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/configuration.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4667 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/exceptions.py
-drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2024-05-06 16:31:52.474550 monei-1.2.5/Monei/model/
--rw-r--r--   0 dmitriy    (501) staff       (20)      339 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/__init__.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    16834 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/activate_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13836 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/address.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12681 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/cancel_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12577 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/cancel_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12780 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/capture_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13897 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    15438 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/confirm_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12743 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/confirm_payment_request_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12843 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/confirm_payment_request_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    23645 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/create_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    17318 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/create_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12357 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/domain_register200_response.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12532 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/error.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12983 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/pause_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    24177 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13516 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_billing_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13224 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_cancellation_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12897 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_customer.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13238 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_last_refund_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13322 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_message_channel.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13501 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_message_language.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    15115 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_next_action.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    14350 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12466 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_payment_method_bizum.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    18413 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12412 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_payment_method_cofidis.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12473 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_payment_method_input.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12409 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_payment_method_paypal.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13795 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_payment_methods.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13206 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_refund_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13122 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_sequence.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13203 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_sequence_recurring.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    17927 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_session_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13579 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_shipping_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12720 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_shop.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13516 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_status.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    18518 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_trace_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13645 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/payment_transaction_type.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    16328 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/recurring_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13130 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/refund_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12531 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/register_domain_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13760 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/send_payment_link_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13791 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/send_payment_receipt_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    23663 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/subscription.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13035 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/subscription_interval.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13388 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/subscription_last_payment.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13038 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/subscription_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    14681 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/subscription_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13377 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/subscription_status.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    17444 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model/update_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    83493 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/model_utils.py
-drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2024-05-06 16:31:52.490919 monei-1.2.5/Monei/models/
--rw-r--r--   0 dmitriy    (501) staff       (20)     5361 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/__init__.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13218 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/activate_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     7862 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/address.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4558 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/cancel_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4753 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/cancel_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4555 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/capture_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     8279 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/models/card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    10729 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/confirm_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4410 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/confirm_payment_request_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5734 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/confirm_payment_request_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    28798 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/create_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    16922 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/create_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4839 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/error.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4192 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/models/inline_object.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4232 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/inline_response200.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4259 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/inline_response2001.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5868 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/pause_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    30026 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     8003 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_billing_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3843 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_cancellation_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5719 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_customer.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3835 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_last_refund_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3752 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_message_channel.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3798 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_message_language.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     8566 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_next_action.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    11314 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4522 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_payment_method_bizum.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4562 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_payment_method_bizum_input.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    17455 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     8968 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_payment_method_card_input.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4418 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_payment_method_cofidis.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5041 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_payment_method_input.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     6326 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_payment_method_klarna.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4522 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_payment_method_mbway.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4410 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_payment_method_paypal.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    11576 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_payment_method_sepa.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4486 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_payment_method_trustly.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3819 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_refund_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5395 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_sequence.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5463 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_sequence_recurring.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    19485 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_session_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     8091 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_shipping_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5068 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_shop.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3951 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_status.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    21011 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_trace_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3777 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/payment_transaction_type.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    12705 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/recurring_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5273 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/refund_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4631 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/register_domain_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     7103 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/send_payment_link_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     7185 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/send_payment_receipt_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5462 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/send_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    31445 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/subscription.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3760 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/subscription_interval.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     6814 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/subscription_last_payment.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5398 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/subscription_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    10663 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/subscription_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3890 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/subscription_status.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    17875 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/update_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     6524 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/models/validate_bizum_phone_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1732 2023-05-26 17:29:18.000000 monei-1.2.5/Monei/monei_client.py
--rw-r--r--   0 dmitriy    (501) staff       (20)    13190 2024-05-06 15:24:12.000000 monei-1.2.5/Monei/rest.py
-drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2024-05-06 16:31:52.501056 monei-1.2.5/Monei.egg-info/
--rw-r--r--   0 dmitriy    (501) staff       (20)      863 2024-05-06 16:31:52.000000 monei-1.2.5/Monei.egg-info/PKG-INFO
--rw-r--r--   0 dmitriy    (501) staff       (20)     7223 2024-05-06 16:31:52.000000 monei-1.2.5/Monei.egg-info/SOURCES.txt
--rw-r--r--   0 dmitriy    (501) staff       (20)        1 2024-05-06 16:31:52.000000 monei-1.2.5/Monei.egg-info/dependency_links.txt
--rw-r--r--   0 dmitriy    (501) staff       (20)       48 2024-05-06 16:31:52.000000 monei-1.2.5/Monei.egg-info/requires.txt
--rw-r--r--   0 dmitriy    (501) staff       (20)        6 2024-05-06 16:31:52.000000 monei-1.2.5/Monei.egg-info/top_level.txt
--rw-r--r--   0 dmitriy    (501) staff       (20)      863 2024-05-06 16:31:52.501343 monei-1.2.5/PKG-INFO
--rw-r--r--   0 dmitriy    (501) staff       (20)     2379 2023-05-26 17:29:15.000000 monei-1.2.5/README.md
--rw-r--r--   0 dmitriy    (501) staff       (20)      128 2024-05-06 16:31:52.501667 monei-1.2.5/setup.cfg
--rw-r--r--   0 dmitriy    (501) staff       (20)     1304 2023-05-26 17:29:15.000000 monei-1.2.5/setup.py
-drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2024-05-06 16:31:52.500875 monei-1.2.5/test/
--rw-r--r--   0 dmitriy    (501) staff       (20)     2539 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_activate_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1699 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_address.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1509 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_apple_pay_domain_api.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1694 2023-09-19 16:45:10.000000 monei-1.2.5/test/test_bizum_api.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1690 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_cancel_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2167 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_cancel_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1680 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_capture_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1583 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3205 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_confirm_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2370 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_confirm_payment_request_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2283 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_confirm_payment_request_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     5396 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_create_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     4226 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_create_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1734 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_domain_register200_response.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1559 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_error.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2021 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_inline_object.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2063 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_inline_response200.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2300 2023-09-19 16:45:09.000000 monei-1.2.5/test/test_inline_response2001.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2198 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_pause_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     6369 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2100 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_billing_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1694 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_cancellation_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1697 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_customer.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1674 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_last_refund_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2314 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_message_channel.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2325 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_message_language.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1779 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_next_action.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2322 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1731 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_payment_method_bizum.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2452 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_payment_method_bizum_input.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1908 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2635 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_payment_method_card_input.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2177 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_payment_method_cofidis.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1897 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_payment_method_input.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2450 2023-09-19 16:45:09.000000 monei-1.2.5/test/test_payment_payment_method_klarna.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2384 2023-09-19 16:45:09.000000 monei-1.2.5/test/test_payment_payment_method_mbway.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1738 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_payment_method_paypal.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2669 2023-09-19 16:45:09.000000 monei-1.2.5/test/test_payment_payment_method_sepa.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2405 2023-09-19 16:45:09.000000 monei-1.2.5/test/test_payment_payment_method_trustly.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1706 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_payment_methods.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1628 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_refund_reason.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1874 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_sequence.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1785 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_sequence_recurring.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2159 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_session_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2111 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_shipping_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1606 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_shop.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1560 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_status.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2219 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_trace_details.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1661 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payment_transaction_type.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1787 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_payments_api.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3401 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_recurring_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     1716 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_refund_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2184 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_register_domain_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2198 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_send_payment_link_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2231 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_send_payment_receipt_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2350 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_send_payment_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     6061 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_subscription.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2065 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_subscription_interval.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2268 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_subscription_last_payment.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2543 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_subscription_payment_method.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2433 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_subscription_payment_method_card.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2043 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_subscription_status.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2268 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_subscriptions_api.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     3994 2023-05-26 17:29:18.000000 monei-1.2.5/test/test_update_subscription_request.py
--rw-r--r--   0 dmitriy    (501) staff       (20)     2647 2023-09-19 16:45:09.000000 monei-1.2.5/test/test_validate_bizum_phone_request.py
+drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2024-05-30 14:03:16.574524 monei-1.2.6/
+drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2024-05-30 14:03:16.547406 monei-1.2.6/Monei/
+-rw-r--r--   0 dmitriy    (501) staff       (20)     6011 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/__init__.py
+drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2024-05-30 14:03:16.548823 monei-1.2.6/Monei/api/
+-rw-r--r--   0 dmitriy    (501) staff       (20)      293 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/api/__init__.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     7936 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/api/apple_pay_domain_api.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     7513 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/api/bizum_api.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    60407 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/api/payments_api.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    40355 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/api/subscriptions_api.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    27077 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/api_client.py
+drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2024-05-30 14:03:16.549229 monei-1.2.6/Monei/apis/
+-rw-r--r--   0 dmitriy    (501) staff       (20)      599 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/apis/__init__.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    14455 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/configuration.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4667 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/exceptions.py
+drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2024-05-30 14:03:16.555827 monei-1.2.6/Monei/model/
+-rw-r--r--   0 dmitriy    (501) staff       (20)      339 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/__init__.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    16834 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/activate_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13836 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/address.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12681 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/cancel_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12577 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/cancel_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12780 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/capture_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13897 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    15438 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/confirm_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12743 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/confirm_payment_request_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12843 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/confirm_payment_request_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    23645 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/create_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    17318 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/create_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12357 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/domain_register200_response.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12532 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/error.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12983 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/pause_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    24177 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13516 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_billing_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13224 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_cancellation_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12897 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_customer.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13238 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_last_refund_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13322 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_message_channel.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13501 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_message_language.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    15115 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_next_action.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    14350 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12466 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_payment_method_bizum.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    18413 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12412 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_payment_method_cofidis.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12473 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_payment_method_input.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12409 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_payment_method_paypal.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13795 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_payment_methods.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13206 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_refund_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13122 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_sequence.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13203 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_sequence_recurring.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    17927 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_session_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13579 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_shipping_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12720 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_shop.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13516 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_status.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    18518 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_trace_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13645 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/payment_transaction_type.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    16328 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/recurring_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13130 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/refund_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12531 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/register_domain_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13760 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/send_payment_link_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13791 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/send_payment_receipt_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    23663 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/subscription.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13035 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/subscription_interval.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13388 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/subscription_last_payment.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13038 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/subscription_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    14681 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/subscription_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13377 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/subscription_status.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    17444 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model/update_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    83493 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/model_utils.py
+drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2024-05-30 14:03:16.565990 monei-1.2.6/Monei/models/
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5361 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/__init__.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13218 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/activate_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     7862 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/address.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4558 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/cancel_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4753 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/cancel_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4555 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/capture_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     8279 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/models/card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    10729 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/confirm_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4410 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/confirm_payment_request_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5734 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/confirm_payment_request_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    29704 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/create_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    16922 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/create_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4839 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/error.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4192 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/models/inline_object.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4232 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/inline_response200.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4259 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/inline_response2001.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5868 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/pause_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    30880 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     8003 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_billing_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3843 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_cancellation_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5719 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_customer.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3835 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_last_refund_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3752 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_message_channel.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3798 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_message_language.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     8566 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_next_action.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    11314 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4522 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_payment_method_bizum.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4562 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_payment_method_bizum_input.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    17455 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     8968 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_payment_method_card_input.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4418 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_payment_method_cofidis.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5041 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_payment_method_input.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     6326 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_payment_method_klarna.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4522 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_payment_method_mbway.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4410 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_payment_method_paypal.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    11576 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_payment_method_sepa.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4486 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_payment_method_trustly.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3819 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_refund_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5395 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_sequence.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5463 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_sequence_recurring.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    19485 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_session_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     8091 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_shipping_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5068 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_shop.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3951 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_status.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    21011 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_trace_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3777 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/payment_transaction_type.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    12705 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/recurring_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5273 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/refund_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4631 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/register_domain_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     7103 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/send_payment_link_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     7185 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/send_payment_receipt_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5462 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/send_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    31445 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/subscription.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3760 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/subscription_interval.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     6814 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/subscription_last_payment.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5398 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/subscription_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    10663 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/subscription_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3890 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/subscription_status.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    17875 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/update_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     6524 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/models/validate_bizum_phone_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1732 2023-05-26 17:29:18.000000 monei-1.2.6/Monei/monei_client.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)    13190 2024-05-30 14:02:56.000000 monei-1.2.6/Monei/rest.py
+drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2024-05-30 14:03:16.574136 monei-1.2.6/Monei.egg-info/
+-rw-r--r--   0 dmitriy    (501) staff       (20)      863 2024-05-30 14:03:16.000000 monei-1.2.6/Monei.egg-info/PKG-INFO
+-rw-r--r--   0 dmitriy    (501) staff       (20)     7223 2024-05-30 14:03:16.000000 monei-1.2.6/Monei.egg-info/SOURCES.txt
+-rw-r--r--   0 dmitriy    (501) staff       (20)        1 2024-05-30 14:03:16.000000 monei-1.2.6/Monei.egg-info/dependency_links.txt
+-rw-r--r--   0 dmitriy    (501) staff       (20)       48 2024-05-30 14:03:16.000000 monei-1.2.6/Monei.egg-info/requires.txt
+-rw-r--r--   0 dmitriy    (501) staff       (20)        6 2024-05-30 14:03:16.000000 monei-1.2.6/Monei.egg-info/top_level.txt
+-rw-r--r--   0 dmitriy    (501) staff       (20)      863 2024-05-30 14:03:16.574448 monei-1.2.6/PKG-INFO
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2379 2023-05-26 17:29:15.000000 monei-1.2.6/README.md
+-rw-r--r--   0 dmitriy    (501) staff       (20)      128 2024-05-30 14:03:16.574751 monei-1.2.6/setup.cfg
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1304 2023-05-26 17:29:15.000000 monei-1.2.6/setup.py
+drwxr-xr-x   0 dmitriy    (501) staff       (20)        0 2024-05-30 14:03:16.573972 monei-1.2.6/test/
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2539 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_activate_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1699 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_address.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1509 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_apple_pay_domain_api.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1694 2023-09-19 16:45:10.000000 monei-1.2.6/test/test_bizum_api.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1690 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_cancel_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2167 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_cancel_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1680 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_capture_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1583 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3205 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_confirm_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2370 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_confirm_payment_request_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2283 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_confirm_payment_request_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     5396 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_create_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     4226 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_create_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1734 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_domain_register200_response.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1559 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_error.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2021 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_inline_object.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2063 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_inline_response200.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2300 2023-09-19 16:45:09.000000 monei-1.2.6/test/test_inline_response2001.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2198 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_pause_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     6369 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2100 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_billing_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1694 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_cancellation_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1697 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_customer.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1674 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_last_refund_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2314 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_message_channel.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2325 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_message_language.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1779 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_next_action.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2322 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1731 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_payment_method_bizum.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2452 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_payment_method_bizum_input.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1908 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2635 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_payment_method_card_input.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2177 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_payment_method_cofidis.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1897 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_payment_method_input.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2450 2023-09-19 16:45:09.000000 monei-1.2.6/test/test_payment_payment_method_klarna.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2384 2023-09-19 16:45:09.000000 monei-1.2.6/test/test_payment_payment_method_mbway.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1738 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_payment_method_paypal.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2669 2023-09-19 16:45:09.000000 monei-1.2.6/test/test_payment_payment_method_sepa.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2405 2023-09-19 16:45:09.000000 monei-1.2.6/test/test_payment_payment_method_trustly.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1706 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_payment_methods.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1628 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_refund_reason.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1874 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_sequence.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1785 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_sequence_recurring.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2159 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_session_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2111 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_shipping_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1606 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_shop.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1560 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_status.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2219 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_trace_details.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1661 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payment_transaction_type.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1787 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_payments_api.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3401 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_recurring_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     1716 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_refund_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2184 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_register_domain_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2198 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_send_payment_link_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2231 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_send_payment_receipt_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2350 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_send_payment_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     6061 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_subscription.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2065 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_subscription_interval.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2268 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_subscription_last_payment.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2543 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_subscription_payment_method.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2433 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_subscription_payment_method_card.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2043 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_subscription_status.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2268 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_subscriptions_api.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     3994 2023-05-26 17:29:18.000000 monei-1.2.6/test/test_update_subscription_request.py
+-rw-r--r--   0 dmitriy    (501) staff       (20)     2647 2023-09-19 16:45:09.000000 monei-1.2.6/test/test_validate_bizum_phone_request.py
```

### Comparing `monei-1.2.5/Monei/__init__.py` & `monei-1.2.6/Monei/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 # flake8: noqa
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.2.5"
+__version__ = "1.2.6"
 
 # import apis into sdk package
 from Monei.api.apple_pay_domain_api import ApplePayDomainApi
 from Monei.api.bizum_api import BizumApi
 from Monei.api.payments_api import PaymentsApi
 from Monei.api.subscriptions_api import SubscriptionsApi
```

#### html2text {}

```diff
@@ -8,17 +8,17 @@
     * _P_H_P_ _S_D_K
     * _P_y_t_h_o_n_ _S_D_K
     * _N_o_d_e_._j_s_ _S_D_K
     * _P_o_s_t_m_a_n
 ****** IImmppoorrttaanntt:: ******
 IIff yyoouu aarree nnoott uussiinngg oouurr ooffffiicciiaall SSDDKKss,, yyoouu nneeeedd ttoo pprroovviiddee aa vvaalliidd UUsseerr--AAggeenntt
 hheeaaddeerr iinn eeaacchh rreeqquueesstt,, ootthheerrwwiissee yyoouurr rreeqquueessttss wwiillll bbee rreejjeecctteedd..
-# noqa: E501 The version of the OpenAPI document: 1.4.4 Generated by: https://
+# noqa: E501 The version of the OpenAPI document: 1.4.6 Generated by: https://
 openapi-generator.tech """ from __future__ import absolute_import __version__ =
-"1.2.5" # import apis into sdk package from Monei.api.apple_pay_domain_api
+"1.2.6" # import apis into sdk package from Monei.api.apple_pay_domain_api
 import ApplePayDomainApi from Monei.api.bizum_api import BizumApi from
 Monei.api.payments_api import PaymentsApi from Monei.api.subscriptions_api
 import SubscriptionsApi # import ApiClient from Monei.api_client import
 ApiClient from Monei.configuration import Configuration from Monei.exceptions
 import OpenApiException from Monei.exceptions import ApiTypeError from
 Monei.exceptions import ApiValueError from Monei.exceptions import ApiKeyError
 from Monei.exceptions import ApiException # import models into sdk package from
```

### Comparing `monei-1.2.5/Monei/api/apple_pay_domain_api.py` & `monei-1.2.6/Monei/api/apple_pay_domain_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/api/bizum_api.py` & `monei-1.2.6/Monei/api/bizum_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/api/payments_api.py` & `monei-1.2.6/Monei/api/payments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/api/subscriptions_api.py` & `monei-1.2.6/Monei/api/subscriptions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/api_client.py` & `monei-1.2.6/Monei/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
 import datetime
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.2.5/python'
+        self.user_agent = 'OpenAPI-Generator/1.2.6/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `monei-1.2.5/Monei/apis/__init__.py` & `monei-1.2.6/Monei/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/configuration.py` & `monei-1.2.6/Monei/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import copy
@@ -354,16 +354,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.4.4\n"\
-               "SDK Package Version: 1.2.5".\
+               "Version of the API: 1.4.6\n"\
+               "SDK Package Version: 1.2.6".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `monei-1.2.5/Monei/exceptions.py` & `monei-1.2.6/Monei/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `monei-1.2.5/Monei/model/activate_subscription_request.py` & `monei-1.2.6/Monei/model/activate_subscription_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/address.py` & `monei-1.2.6/Monei/model/address.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/cancel_payment_request.py` & `monei-1.2.6/Monei/model/cancel_payment_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/cancel_subscription_request.py` & `monei-1.2.6/Monei/model/cancel_subscription_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/capture_payment_request.py` & `monei-1.2.6/Monei/model/capture_payment_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/card.py` & `monei-1.2.6/Monei/model/card.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/confirm_payment_request.py` & `monei-1.2.6/Monei/model/confirm_payment_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/confirm_payment_request_payment_method.py` & `monei-1.2.6/Monei/model/confirm_payment_request_payment_method.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/confirm_payment_request_payment_method_card.py` & `monei-1.2.6/Monei/model/confirm_payment_request_payment_method_card.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/create_payment_request.py` & `monei-1.2.6/Monei/model/create_payment_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/create_subscription_request.py` & `monei-1.2.6/Monei/model/create_subscription_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/domain_register200_response.py` & `monei-1.2.6/Monei/model/domain_register200_response.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/error.py` & `monei-1.2.6/Monei/model/error.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/pause_subscription_request.py` & `monei-1.2.6/Monei/model/pause_subscription_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment.py` & `monei-1.2.6/Monei/model/payment.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_billing_details.py` & `monei-1.2.6/Monei/model/payment_billing_details.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_cancellation_reason.py` & `monei-1.2.6/Monei/model/payment_cancellation_reason.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_customer.py` & `monei-1.2.6/Monei/model/payment_customer.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_last_refund_reason.py` & `monei-1.2.6/Monei/model/payment_last_refund_reason.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_message_channel.py` & `monei-1.2.6/Monei/model/payment_message_channel.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_message_language.py` & `monei-1.2.6/Monei/model/payment_message_language.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_next_action.py` & `monei-1.2.6/Monei/model/payment_next_action.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_payment_method.py` & `monei-1.2.6/Monei/model/payment_payment_method.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_payment_method_bizum.py` & `monei-1.2.6/Monei/model/payment_payment_method_bizum.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_payment_method_card.py` & `monei-1.2.6/Monei/model/payment_payment_method_card.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_payment_method_cofidis.py` & `monei-1.2.6/Monei/model/payment_payment_method_cofidis.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_payment_method_input.py` & `monei-1.2.6/Monei/model/payment_payment_method_input.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_payment_method_paypal.py` & `monei-1.2.6/Monei/model/payment_payment_method_paypal.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_payment_methods.py` & `monei-1.2.6/Monei/model/payment_payment_methods.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_refund_reason.py` & `monei-1.2.6/Monei/model/payment_refund_reason.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_sequence.py` & `monei-1.2.6/Monei/model/payment_sequence.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_sequence_recurring.py` & `monei-1.2.6/Monei/model/payment_sequence_recurring.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_session_details.py` & `monei-1.2.6/Monei/model/payment_session_details.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_shipping_details.py` & `monei-1.2.6/Monei/model/payment_shipping_details.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_shop.py` & `monei-1.2.6/Monei/model/payment_shop.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_status.py` & `monei-1.2.6/Monei/model/payment_status.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_trace_details.py` & `monei-1.2.6/Monei/model/payment_trace_details.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/payment_transaction_type.py` & `monei-1.2.6/Monei/model/payment_transaction_type.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/recurring_payment_request.py` & `monei-1.2.6/Monei/model/recurring_payment_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/refund_payment_request.py` & `monei-1.2.6/Monei/model/refund_payment_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/register_domain_request.py` & `monei-1.2.6/Monei/model/register_domain_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/send_payment_link_request.py` & `monei-1.2.6/Monei/model/send_payment_link_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/send_payment_receipt_request.py` & `monei-1.2.6/Monei/model/send_payment_receipt_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/subscription.py` & `monei-1.2.6/Monei/model/subscription.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/subscription_interval.py` & `monei-1.2.6/Monei/model/subscription_interval.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/subscription_last_payment.py` & `monei-1.2.6/Monei/model/subscription_last_payment.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/subscription_payment_method.py` & `monei-1.2.6/Monei/model/subscription_payment_method.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/subscription_payment_method_card.py` & `monei-1.2.6/Monei/model/subscription_payment_method_card.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/subscription_status.py` & `monei-1.2.6/Monei/model/subscription_status.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model/update_subscription_request.py` & `monei-1.2.6/Monei/model/update_subscription_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/model_utils.py` & `monei-1.2.6/Monei/model_utils.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/models/__init__.py` & `monei-1.2.6/Monei/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # import models into model package
```

#### html2text {}

```diff
@@ -8,15 +8,15 @@
     * _P_H_P_ _S_D_K
     * _P_y_t_h_o_n_ _S_D_K
     * _N_o_d_e_._j_s_ _S_D_K
     * _P_o_s_t_m_a_n
 ****** IImmppoorrttaanntt:: ******
 IIff yyoouu aarree nnoott uussiinngg oouurr ooffffiicciiaall SSDDKKss,, yyoouu nneeeedd ttoo pprroovviiddee aa vvaalliidd UUsseerr--AAggeenntt
 hheeaaddeerr iinn eeaacchh rreeqquueesstt,, ootthheerrwwiissee yyoouurr rreeqquueessttss wwiillll bbee rreejjeecctteedd..
-# noqa: E501 The version of the OpenAPI document: 1.4.4 Generated by: https://
+# noqa: E501 The version of the OpenAPI document: 1.4.6 Generated by: https://
 openapi-generator.tech """ from __future__ import absolute_import # import
 models into model package from Monei.models.activate_subscription_request
 import ActivateSubscriptionRequest from Monei.models.address import Address
 from Monei.models.cancel_payment_request import CancelPaymentRequest from
 Monei.models.cancel_subscription_request import CancelSubscriptionRequest from
 Monei.models.capture_payment_request import CapturePaymentRequest from
 Monei.models.confirm_payment_request import ConfirmPaymentRequest from
```

### Comparing `monei-1.2.5/Monei/models/activate_subscription_request.py` & `monei-1.2.6/Monei/models/activate_subscription_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/address.py` & `monei-1.2.6/Monei/models/address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/cancel_payment_request.py` & `monei-1.2.6/Monei/models/cancel_payment_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/cancel_subscription_request.py` & `monei-1.2.6/Monei/models/cancel_subscription_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/capture_payment_request.py` & `monei-1.2.6/Monei/models/capture_payment_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/card.py` & `monei-1.2.6/Monei/models/card.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/models/confirm_payment_request.py` & `monei-1.2.6/Monei/models/confirm_payment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/confirm_payment_request_payment_method.py` & `monei-1.2.6/Monei/models/confirm_payment_request_payment_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/confirm_payment_request_payment_method_card.py` & `monei-1.2.6/Monei/models/confirm_payment_request_payment_method_card.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/create_payment_request.py` & `monei-1.2.6/Monei/models/create_payment_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -43,14 +43,15 @@
         'payment_token': 'str',
         'session_id': 'str',
         'generate_payment_token': 'bool',
         'payment_method': 'PaymentPaymentMethodInput',
         'allowed_payment_methods': 'PaymentPaymentMethods',
         'transaction_type': 'PaymentTransactionType',
         'sequence': 'PaymentSequence',
+        'store_id': 'str',
         'point_of_sale_id': 'str',
         'subscription_id': 'str',
         'auto_recover': 'bool',
         'description': 'str',
         'customer': 'PaymentCustomer',
         'billing_details': 'PaymentBillingDetails',
         'shipping_details': 'PaymentShippingDetails',
@@ -70,27 +71,28 @@
         'payment_token': 'paymentToken',
         'session_id': 'sessionId',
         'generate_payment_token': 'generatePaymentToken',
         'payment_method': 'paymentMethod',
         'allowed_payment_methods': 'allowedPaymentMethods',
         'transaction_type': 'transactionType',
         'sequence': 'sequence',
+        'store_id': 'storeId',
         'point_of_sale_id': 'pointOfSaleId',
         'subscription_id': 'subscriptionId',
         'auto_recover': 'autoRecover',
         'description': 'description',
         'customer': 'customer',
         'billing_details': 'billingDetails',
         'shipping_details': 'shippingDetails',
         'session_details': 'sessionDetails',
         'expire_at': 'expireAt',
         'metadata': 'metadata'
     }
 
-    def __init__(self, amount=None, currency=None, order_id=None, callback_url=None, complete_url=None, fail_url=None, cancel_url=None, payment_token=None, session_id=None, generate_payment_token=False, payment_method=None, allowed_payment_methods=None, transaction_type=None, sequence=None, point_of_sale_id=None, subscription_id=None, auto_recover=None, description=None, customer=None, billing_details=None, shipping_details=None, session_details=None, expire_at=None, metadata=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, amount=None, currency=None, order_id=None, callback_url=None, complete_url=None, fail_url=None, cancel_url=None, payment_token=None, session_id=None, generate_payment_token=False, payment_method=None, allowed_payment_methods=None, transaction_type=None, sequence=None, store_id=None, point_of_sale_id=None, subscription_id=None, auto_recover=None, description=None, customer=None, billing_details=None, shipping_details=None, session_details=None, expire_at=None, metadata=None, local_vars_configuration=None):  # noqa: E501
         """CreatePaymentRequest - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._amount = None
         self._currency = None
@@ -102,14 +104,15 @@
         self._payment_token = None
         self._session_id = None
         self._generate_payment_token = None
         self._payment_method = None
         self._allowed_payment_methods = None
         self._transaction_type = None
         self._sequence = None
+        self._store_id = None
         self._point_of_sale_id = None
         self._subscription_id = None
         self._auto_recover = None
         self._description = None
         self._customer = None
         self._billing_details = None
         self._shipping_details = None
@@ -139,14 +142,16 @@
             self.payment_method = payment_method
         if allowed_payment_methods is not None:
             self.allowed_payment_methods = allowed_payment_methods
         if transaction_type is not None:
             self.transaction_type = transaction_type
         if sequence is not None:
             self.sequence = sequence
+        if store_id is not None:
+            self.store_id = store_id
         if point_of_sale_id is not None:
             self.point_of_sale_id = point_of_sale_id
         if subscription_id is not None:
             self.subscription_id = subscription_id
         if auto_recover is not None:
             self.auto_recover = auto_recover
         if description is not None:
@@ -481,14 +486,37 @@
         :param sequence: The sequence of this CreatePaymentRequest.  # noqa: E501
         :type: PaymentSequence
         """
 
         self._sequence = sequence
 
     @property
+    def store_id(self):
+        """Gets the store_id of this CreatePaymentRequest.  # noqa: E501
+
+        A unique identifier of the Store. If specified the payment is attached to this Store.   # noqa: E501
+
+        :return: The store_id of this CreatePaymentRequest.  # noqa: E501
+        :rtype: str
+        """
+        return self._store_id
+
+    @store_id.setter
+    def store_id(self, store_id):
+        """Sets the store_id of this CreatePaymentRequest.
+
+        A unique identifier of the Store. If specified the payment is attached to this Store.   # noqa: E501
+
+        :param store_id: The store_id of this CreatePaymentRequest.  # noqa: E501
+        :type: str
+        """
+
+        self._store_id = store_id
+
+    @property
     def point_of_sale_id(self):
         """Gets the point_of_sale_id of this CreatePaymentRequest.  # noqa: E501
 
         A unique identifier of the Point of Sale. If specified the payment is attached to this Point of Sale. If there is a QR code attached to the same Point of Sale, this payment will be available by scanning the QR code.   # noqa: E501
 
         :return: The point_of_sale_id of this CreatePaymentRequest.  # noqa: E501
         :rtype: str
```

### Comparing `monei-1.2.5/Monei/models/create_subscription_request.py` & `monei-1.2.6/Monei/models/create_subscription_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/error.py` & `monei-1.2.6/Monei/models/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/inline_object.py` & `monei-1.2.6/Monei/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/models/inline_response200.py` & `monei-1.2.6/Monei/models/inline_response200.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/inline_response2001.py` & `monei-1.2.6/Monei/models/inline_response2001.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/pause_subscription_request.py` & `monei-1.2.6/Monei/models/pause_subscription_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment.py` & `monei-1.2.6/Monei/models/payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
 
@@ -54,14 +54,15 @@
         'cancellation_reason': 'PaymentCancellationReason',
         'session_details': 'PaymentSessionDetails',
         'trace_details': 'PaymentTraceDetails',
         'payment_token': 'str',
         'payment_method': 'PaymentPaymentMethod',
         'sequence': 'PaymentSequence',
         'sequence_id': 'str',
+        'store_id': 'str',
         'point_of_sale_id': 'str',
         'metadata': 'object',
         'next_action': 'PaymentNextAction',
         'created_at': 'int',
         'updated_at': 'int'
     }
 
@@ -87,22 +88,23 @@
         'cancellation_reason': 'cancellationReason',
         'session_details': 'sessionDetails',
         'trace_details': 'traceDetails',
         'payment_token': 'paymentToken',
         'payment_method': 'paymentMethod',
         'sequence': 'sequence',
         'sequence_id': 'sequenceId',
+        'store_id': 'storeId',
         'point_of_sale_id': 'pointOfSaleId',
         'metadata': 'metadata',
         'next_action': 'nextAction',
         'created_at': 'createdAt',
         'updated_at': 'updatedAt'
     }
 
-    def __init__(self, id=None, amount=None, currency=None, order_id=None, description=None, account_id=None, authorization_code=None, livemode=None, status=None, status_code=None, status_message=None, customer=None, shop=None, billing_details=None, shipping_details=None, refunded_amount=None, last_refund_amount=None, last_refund_reason=None, cancellation_reason=None, session_details=None, trace_details=None, payment_token=None, payment_method=None, sequence=None, sequence_id=None, point_of_sale_id=None, metadata=None, next_action=None, created_at=None, updated_at=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, amount=None, currency=None, order_id=None, description=None, account_id=None, authorization_code=None, livemode=None, status=None, status_code=None, status_message=None, customer=None, shop=None, billing_details=None, shipping_details=None, refunded_amount=None, last_refund_amount=None, last_refund_reason=None, cancellation_reason=None, session_details=None, trace_details=None, payment_token=None, payment_method=None, sequence=None, sequence_id=None, store_id=None, point_of_sale_id=None, metadata=None, next_action=None, created_at=None, updated_at=None, local_vars_configuration=None):  # noqa: E501
         """Payment - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._amount = None
@@ -125,14 +127,15 @@
         self._cancellation_reason = None
         self._session_details = None
         self._trace_details = None
         self._payment_token = None
         self._payment_method = None
         self._sequence = None
         self._sequence_id = None
+        self._store_id = None
         self._point_of_sale_id = None
         self._metadata = None
         self._next_action = None
         self._created_at = None
         self._updated_at = None
         self.discriminator = None
 
@@ -182,14 +185,16 @@
             self.payment_token = payment_token
         if payment_method is not None:
             self.payment_method = payment_method
         if sequence is not None:
             self.sequence = sequence
         if sequence_id is not None:
             self.sequence_id = sequence_id
+        if store_id is not None:
+            self.store_id = store_id
         if point_of_sale_id is not None:
             self.point_of_sale_id = point_of_sale_id
         if metadata is not None:
             self.metadata = metadata
         if next_action is not None:
             self.next_action = next_action
         if created_at is not None:
@@ -747,14 +752,37 @@
         :param sequence_id: The sequence_id of this Payment.  # noqa: E501
         :type: str
         """
 
         self._sequence_id = sequence_id
 
     @property
+    def store_id(self):
+        """Gets the store_id of this Payment.  # noqa: E501
+
+        A unique identifier of the Store. If specified the payment is attached to this Store.   # noqa: E501
+
+        :return: The store_id of this Payment.  # noqa: E501
+        :rtype: str
+        """
+        return self._store_id
+
+    @store_id.setter
+    def store_id(self, store_id):
+        """Sets the store_id of this Payment.
+
+        A unique identifier of the Store. If specified the payment is attached to this Store.   # noqa: E501
+
+        :param store_id: The store_id of this Payment.  # noqa: E501
+        :type: str
+        """
+
+        self._store_id = store_id
+
+    @property
     def point_of_sale_id(self):
         """Gets the point_of_sale_id of this Payment.  # noqa: E501
 
         A unique identifier of the Point of Sale. If specified the payment is attached to this Point of Sale. If there is a QR code attached to the same Point of Sale, this payment will be available by scanning the QR code.   # noqa: E501
 
         :return: The point_of_sale_id of this Payment.  # noqa: E501
         :rtype: str
```

### Comparing `monei-1.2.5/Monei/models/payment_billing_details.py` & `monei-1.2.6/Monei/models/payment_billing_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_cancellation_reason.py` & `monei-1.2.6/Monei/models/payment_cancellation_reason.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_customer.py` & `monei-1.2.6/Monei/models/payment_customer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_last_refund_reason.py` & `monei-1.2.6/Monei/models/payment_last_refund_reason.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_message_channel.py` & `monei-1.2.6/Monei/models/payment_message_channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_message_language.py` & `monei-1.2.6/Monei/models/payment_message_language.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_next_action.py` & `monei-1.2.6/Monei/models/payment_next_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_payment_method.py` & `monei-1.2.6/Monei/models/payment_payment_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_payment_method_bizum.py` & `monei-1.2.6/Monei/models/payment_payment_method_bizum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_payment_method_bizum_input.py` & `monei-1.2.6/Monei/models/payment_payment_method_bizum_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_payment_method_card.py` & `monei-1.2.6/Monei/models/payment_payment_method_card.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_payment_method_card_input.py` & `monei-1.2.6/Monei/models/payment_payment_method_card_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_payment_method_cofidis.py` & `monei-1.2.6/Monei/models/payment_payment_method_cofidis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_payment_method_input.py` & `monei-1.2.6/Monei/models/payment_payment_method_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_payment_method_klarna.py` & `monei-1.2.6/Monei/models/payment_payment_method_klarna.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_payment_method_mbway.py` & `monei-1.2.6/Monei/models/payment_payment_method_mbway.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_payment_method_paypal.py` & `monei-1.2.6/Monei/models/payment_payment_method_paypal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_payment_method_sepa.py` & `monei-1.2.6/Monei/models/payment_payment_method_sepa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_payment_method_trustly.py` & `monei-1.2.6/Monei/models/payment_payment_method_trustly.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_refund_reason.py` & `monei-1.2.6/Monei/models/payment_refund_reason.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_sequence.py` & `monei-1.2.6/Monei/models/payment_sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_sequence_recurring.py` & `monei-1.2.6/Monei/models/payment_sequence_recurring.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_session_details.py` & `monei-1.2.6/Monei/models/payment_session_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_shipping_details.py` & `monei-1.2.6/Monei/models/payment_shipping_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_shop.py` & `monei-1.2.6/Monei/models/payment_shop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_status.py` & `monei-1.2.6/Monei/models/payment_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_trace_details.py` & `monei-1.2.6/Monei/models/payment_trace_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/payment_transaction_type.py` & `monei-1.2.6/Monei/models/payment_transaction_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/recurring_payment_request.py` & `monei-1.2.6/Monei/models/recurring_payment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/refund_payment_request.py` & `monei-1.2.6/Monei/models/refund_payment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/register_domain_request.py` & `monei-1.2.6/Monei/models/register_domain_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/send_payment_link_request.py` & `monei-1.2.6/Monei/models/send_payment_link_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/send_payment_receipt_request.py` & `monei-1.2.6/Monei/models/send_payment_receipt_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/send_payment_request.py` & `monei-1.2.6/Monei/models/send_payment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/subscription.py` & `monei-1.2.6/Monei/models/subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/subscription_interval.py` & `monei-1.2.6/Monei/models/subscription_interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/subscription_last_payment.py` & `monei-1.2.6/Monei/models/subscription_last_payment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/subscription_payment_method.py` & `monei-1.2.6/Monei/models/subscription_payment_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/subscription_payment_method_card.py` & `monei-1.2.6/Monei/models/subscription_payment_method_card.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/subscription_status.py` & `monei-1.2.6/Monei/models/subscription_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/update_subscription_request.py` & `monei-1.2.6/Monei/models/update_subscription_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/models/validate_bizum_phone_request.py` & `monei-1.2.6/Monei/models/validate_bizum_phone_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import pprint
 import re  # noqa: F401
```

### Comparing `monei-1.2.5/Monei/monei_client.py` & `monei-1.2.6/Monei/monei_client.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/Monei/rest.py` & `monei-1.2.6/Monei/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     MONEI API v1
 
     <p>The MONEI API is organized around <a href=\"https://en.wikipedia.org/wiki/Representational_State_Transfer\">REST</a>. Our API has predictable resource-oriented URLs, accepts JSON-encoded request bodies, returns JSON-encoded responses, and uses standard HTTP response codes, authentication, and verbs.</p> <h4 id=\"base-url\">Base URL:</h4> <p><a href=\"https://api.monei.com/v1\">https://api.monei.com/v1</a></p> <h4 id=\"client-libraries\">Client libraries:</h4> <ul> <li><a href=\"https://github.com/MONEI/monei-php-sdk\">PHP SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-python-sdk\">Python SDK</a></li> <li><a href=\"https://github.com/MONEI/monei-node-sdk\">Node.js SDK</a></li> <li><a href=\"https://postman.monei.com/\">Postman</a></li> </ul> <h4 id=\"important\">Important:</h4> <p><strong>If you are not using our official SDKs, you need to provide a valid <code>User-Agent</code> header in each request, otherwise your requests will be rejected.</strong></p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.4.4
+    The version of the OpenAPI document: 1.4.6
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 import io
```

### Comparing `monei-1.2.5/Monei.egg-info/SOURCES.txt` & `monei-1.2.6/Monei.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/README.md` & `monei-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/setup.py` & `monei-1.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_activate_subscription_request.py` & `monei-1.2.6/test/test_activate_subscription_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_address.py` & `monei-1.2.6/test/test_address.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_apple_pay_domain_api.py` & `monei-1.2.6/test/test_apple_pay_domain_api.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_bizum_api.py` & `monei-1.2.6/test/test_bizum_api.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_cancel_payment_request.py` & `monei-1.2.6/test/test_cancel_payment_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_cancel_subscription_request.py` & `monei-1.2.6/test/test_cancel_subscription_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_capture_payment_request.py` & `monei-1.2.6/test/test_capture_payment_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_card.py` & `monei-1.2.6/test/test_card.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_confirm_payment_request.py` & `monei-1.2.6/test/test_confirm_payment_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_confirm_payment_request_payment_method.py` & `monei-1.2.6/test/test_confirm_payment_request_payment_method.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_confirm_payment_request_payment_method_card.py` & `monei-1.2.6/test/test_confirm_payment_request_payment_method_card.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_create_payment_request.py` & `monei-1.2.6/test/test_create_payment_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_create_subscription_request.py` & `monei-1.2.6/test/test_create_subscription_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_domain_register200_response.py` & `monei-1.2.6/test/test_domain_register200_response.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_error.py` & `monei-1.2.6/test/test_error.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_inline_object.py` & `monei-1.2.6/test/test_inline_object.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_inline_response200.py` & `monei-1.2.6/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_inline_response2001.py` & `monei-1.2.6/test/test_inline_response2001.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_pause_subscription_request.py` & `monei-1.2.6/test/test_pause_subscription_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment.py` & `monei-1.2.6/test/test_payment.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_billing_details.py` & `monei-1.2.6/test/test_payment_billing_details.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_cancellation_reason.py` & `monei-1.2.6/test/test_payment_cancellation_reason.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_customer.py` & `monei-1.2.6/test/test_payment_customer.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_last_refund_reason.py` & `monei-1.2.6/test/test_payment_last_refund_reason.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_message_channel.py` & `monei-1.2.6/test/test_payment_message_channel.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_message_language.py` & `monei-1.2.6/test/test_payment_message_language.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_next_action.py` & `monei-1.2.6/test/test_payment_next_action.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_payment_method.py` & `monei-1.2.6/test/test_payment_payment_method.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_payment_method_bizum.py` & `monei-1.2.6/test/test_payment_payment_method_bizum.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_payment_method_bizum_input.py` & `monei-1.2.6/test/test_payment_payment_method_bizum_input.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_payment_method_card.py` & `monei-1.2.6/test/test_payment_payment_method_card.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_payment_method_card_input.py` & `monei-1.2.6/test/test_payment_payment_method_card_input.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_payment_method_cofidis.py` & `monei-1.2.6/test/test_payment_payment_method_cofidis.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_payment_method_input.py` & `monei-1.2.6/test/test_payment_payment_method_input.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_payment_method_klarna.py` & `monei-1.2.6/test/test_payment_payment_method_klarna.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_payment_method_mbway.py` & `monei-1.2.6/test/test_payment_payment_method_mbway.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_payment_method_paypal.py` & `monei-1.2.6/test/test_payment_payment_method_paypal.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_payment_method_sepa.py` & `monei-1.2.6/test/test_payment_payment_method_sepa.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_payment_method_trustly.py` & `monei-1.2.6/test/test_payment_payment_method_trustly.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_payment_methods.py` & `monei-1.2.6/test/test_payment_payment_methods.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_refund_reason.py` & `monei-1.2.6/test/test_payment_refund_reason.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_sequence.py` & `monei-1.2.6/test/test_payment_sequence.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_sequence_recurring.py` & `monei-1.2.6/test/test_payment_sequence_recurring.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_session_details.py` & `monei-1.2.6/test/test_payment_session_details.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_shipping_details.py` & `monei-1.2.6/test/test_payment_shipping_details.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_shop.py` & `monei-1.2.6/test/test_payment_shop.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_status.py` & `monei-1.2.6/test/test_payment_status.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_trace_details.py` & `monei-1.2.6/test/test_payment_trace_details.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payment_transaction_type.py` & `monei-1.2.6/test/test_payment_transaction_type.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_payments_api.py` & `monei-1.2.6/test/test_payments_api.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_recurring_payment_request.py` & `monei-1.2.6/test/test_recurring_payment_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_refund_payment_request.py` & `monei-1.2.6/test/test_refund_payment_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_register_domain_request.py` & `monei-1.2.6/test/test_register_domain_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_send_payment_link_request.py` & `monei-1.2.6/test/test_send_payment_link_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_send_payment_receipt_request.py` & `monei-1.2.6/test/test_send_payment_receipt_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_send_payment_request.py` & `monei-1.2.6/test/test_send_payment_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_subscription.py` & `monei-1.2.6/test/test_subscription.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_subscription_interval.py` & `monei-1.2.6/test/test_subscription_interval.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_subscription_last_payment.py` & `monei-1.2.6/test/test_subscription_last_payment.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_subscription_payment_method.py` & `monei-1.2.6/test/test_subscription_payment_method.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_subscription_payment_method_card.py` & `monei-1.2.6/test/test_subscription_payment_method_card.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_subscription_status.py` & `monei-1.2.6/test/test_subscription_status.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_subscriptions_api.py` & `monei-1.2.6/test/test_subscriptions_api.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_update_subscription_request.py` & `monei-1.2.6/test/test_update_subscription_request.py`

 * *Files identical despite different names*

### Comparing `monei-1.2.5/test/test_validate_bizum_phone_request.py` & `monei-1.2.6/test/test_validate_bizum_phone_request.py`

 * *Files identical despite different names*

