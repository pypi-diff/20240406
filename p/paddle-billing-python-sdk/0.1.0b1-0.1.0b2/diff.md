# Comparing `tmp/paddle-billing-python-sdk-0.1.0b1.tar.gz` & `tmp/paddle-billing-python-sdk-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddle-billing-python-sdk-0.1.0b1.tar", last modified: Mon Feb 26 21:07:51 2024, max compression
+gzip compressed data, was "paddle-billing-python-sdk-0.1.0b2.tar", last modified: Mon Mar  4 22:09:11 2024, max compression
```

## Comparing `paddle-billing-python-sdk-0.1.0b1.tar` & `paddle-billing-python-sdk-0.1.0b2.tar`

### file list

```diff
@@ -1,618 +1,618 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.664469 paddle-billing-python-sdk-0.1.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-02-26 21:07:51.664469 paddle-billing-python-sdk-0.1.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.584469 paddle-billing-python-sdk-0.1.0b1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/examples/catalog_management.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/examples/event_polling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/examples/get_products.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/examples/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.584469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/
--rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/ConditionallyRemoveImportMeta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.588469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Address.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Adjustment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.588469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Adjustments/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Adjustments/AdjustmentCustomerBalance.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Adjustments/AdjustmentItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Adjustments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Business.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.592469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/AddressCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/AdjustmentCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/BusinessCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/Collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/CreditBalanceCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/CustomerCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/DiscountCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/EventCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/EventTypeCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/NotificationCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/NotificationLogCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/NotificationSettingCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/Paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/PriceCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/ProductCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/ReportCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/SubscriptionCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/SubscriptionPreviewCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/TransactionCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/TransactionPreviewCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/TransactionsDataCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/CreditBalance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/DateTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Discount.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.592469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Discounts/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Discounts/DiscountStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Discounts/DiscountType.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Discounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Event.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/EventType.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.596469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Events/
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Events/EventTypeName.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Notification.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/NotificationLog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/NotificationSetting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.596469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/NotificationSettings/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/NotificationSettings/NotificationSettingType.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/NotificationSettings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.596469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Notifications/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Notifications/NotificationOrigin.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Notifications/NotificationPayout.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Notifications/NotificationPayoutStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Notifications/NotificationStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Price.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/PricePreview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.596469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/PricingPreviews/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/PricingPreviews/PricePreviewDetails.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/PricingPreviews/PricePreviewDiscounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/PricingPreviews/PricePreviewItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/PricingPreviews/PricePreviewLineItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/PricingPreviews/PricePreviewTotalsFormatted.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/PricingPreviews/PricePreviewUnitTotalsFormatted.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/PricingPreviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Report.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/ReportCSV.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.596469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Reports/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Reports/ReportFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Reports/ReportFilterName.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Reports/ReportFilterOperator.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Reports/ReportStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Reports/ReportType.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.604469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/Action.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/AddressPreview.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/AdjustmentItemTotals.py
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/AdjustmentProration.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/AdjustmentStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/AdjustmentTimePeriod.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/AdjustmentTotals.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/AdjustmentType.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/AvailablePaymentMethods.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/BillingDetails.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/BillingDetailsUpdate.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/CatalogType.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/ChargebackFee.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/Checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/CollectionMode.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/Contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/CountryCode.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/CurrencyCode.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/CurrencyCodeAdjustments.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/CurrencyCodePayouts.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/CustomData.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/Data.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/ImportMeta.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/Interval.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/Meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/MetaPaginated.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/MethodDetails.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/Money.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/Original.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/Pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/PaymentAttemptStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/PaymentMethodType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/PayoutTotalsAdjustment.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/PriceQuantity.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/Status.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TaxCategory.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TaxMode.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TaxRatesUsed.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TimePeriod.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/Totals.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TransactionDetailsPreview.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TransactionLineItemPreview.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TransactionOrigin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TransactionPaymentAttempt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TransactionPayoutTotals.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TransactionPayoutTotalsAdjusted.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TransactionStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TransactionTotals.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TransactionTotalsAdjusted.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/UnitPriceOverride.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/UnitTotals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/SubscriptionPreview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.608469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionAdjustmentItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionAdjustmentPreview.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionCharge.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionCredit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionDetails.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionDiscount.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionEffectiveFrom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionItemStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionItems.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionItemsWithPrice.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionManagementUrls.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionNextTransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionNonCatalogPrice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionNonCatalogPriceWithProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionNonCatalogProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionOnPaymentFailure.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionPreviewSubscriptionUpdateSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionPrice.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionProration.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionProrationBillingMode.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionResultAction.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionResumeEffectiveFrom.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionScheduledChange.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionScheduledChangeAction.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionTimePeriod.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionTransactionItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionTransactionLineItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionUpdateItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/TransactionData.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/TransactionPreview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.612469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionAdjustmentsTotals.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionBreakdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionCardType.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionCreateItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionCreateItemWithPrice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionDetails.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionItemPreviewWithNonCatalogPrice.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionItemPreviewWithPrice.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionItemPreviewWithPriceId.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionLineItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionNonCatalogPrice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionNonCatalogPriceWithProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionNonCatalogProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionProration.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionTimePeriod.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionUpdateTransactionItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/EnumStringify.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.612469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/ApiError.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.616469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/ApiErrors/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/ApiErrors/AddressApiError.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/ApiErrors/AdjustmentApiError.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/ApiErrors/BusinessApiError.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/ApiErrors/CustomerApiError.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/ApiErrors/DiscountApiError.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/ApiErrors/PriceApiError.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/ApiErrors/ProductApiError.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/ApiErrors/SubscriptionApiError.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/ApiErrors/TransactionApiError.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/ApiErrors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/FieldError.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/SdkException.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.616469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/SdkExceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/SdkExceptions/InvalidArgumentException.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/SdkExceptions/MalformedResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/SdkExceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/FiltersNone.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/FiltersUndefined.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/HasParameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.616469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Logger/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Logger/Formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Logger/NullHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Logger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.616469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.620469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Address.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Adjustment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.620469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Adjustments/
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Adjustments/AdjustmentItem.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Adjustments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Business.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.620469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Businesses/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Businesses/BusinessesContacts.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Businesses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/DateTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Discount.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.620469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Discounts/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Discounts/DiscountStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Discounts/DiscountType.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Discounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Payout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.620469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Payouts/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Payouts/PayoutStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Payouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Price.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.620469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Reports/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Reports/ReportFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Reports/ReportFilterName.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Reports/ReportFilterOperator.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Reports/ReportStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Reports/ReportType.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.628469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/Action.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/AddressPreview.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/AdjustmentItemTotals.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/AdjustmentProration.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/AdjustmentStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/AdjustmentTimePeriod.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/AdjustmentTotals.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/AdjustmentType.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/AvailablePaymentMethods.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/BillingDetails.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/Card.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/CatalogType.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/ChargebackFee.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/Checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/CollectionMode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/CountryCode.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/CurrencyCode.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/CurrencyCodeAdjustments.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/CurrencyCodePayouts.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/CustomData.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/Data.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/ImportMeta.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/Interval.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/MethodDetails.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/Money.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/Original.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/PaymentAttemptStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/PaymentMethodType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/PayoutTotalsAdjustment.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/PriceQuantity.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/Status.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/TaxCategory.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/TaxMode.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/TaxRatesUsed.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/TimePeriod.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/Totals.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/TransactionOrigin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/TransactionPaymentAttempt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/TransactionPayoutTotals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/TransactionPayoutTotalsAdjusted.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/TransactionStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/TransactionTotals.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/TransactionTotalsAdjusted.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/UnitPriceOverride.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/UnitTotals.py
--rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.632469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionAdjustmentItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionCharge.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionCredit.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionDiscount.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionEffectiveFrom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionItemStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionOnPaymentFailure.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionPrice.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionScheduledChange.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionScheduledChangeAction.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionStatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionTimePeriod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.632469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transactions/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transactions/TransactionAdjustmentsTotals.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transactions/TransactionBreakdown.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transactions/TransactionCardType.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transactions/TransactionDetails.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transactions/TransactionItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transactions/TransactionLineItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transactions/TransactionProration.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transactions/TransactionTimePeriod.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.636469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/AddressCreated.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/AddressUpdated.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/AdjustmentCreated.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/AdjustmentUpdated.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/BusinessCreated.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/BusinessUpdated.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/CustomerCreated.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/CustomerUpdated.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/DiscountCreated.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/DiscountImported.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/DiscountUpdated.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/PayoutCreated.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/PayoutPaid.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/PriceCreated.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/PriceUpdated.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/ProductCreated.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/ProductUpdated.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/ReportCreated.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/ReportUpdated.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/SubscriptionActivated.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/SubscriptionCanceled.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/SubscriptionCreated.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/SubscriptionImported.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/SubscriptionPastDue.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/SubscriptionPaused.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/SubscriptionResumed.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/SubscriptionTrialing.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/SubscriptionUpdated.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/TransactionBilled.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/TransactionCanceled.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/TransactionCompleted.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/TransactionCreated.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/TransactionPaid.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/TransactionPastDue.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/TransactionPaymentFailed.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/TransactionReady.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/TransactionUpdated.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/PaddleSignature.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Verifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/PaddleStrEnum.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/RecursivelyRemoveKey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.636469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.636469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Addresses/
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Addresses/AddressesClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.640469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Addresses/Operations/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Addresses/Operations/CreateAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Addresses/Operations/ListAddresses.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Addresses/Operations/UpdateAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Addresses/Operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Addresses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.640469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Adjustments/
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Adjustments/AdjustmentsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.640469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Adjustments/Operations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.640469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Adjustments/Operations/Create/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Adjustments/Operations/Create/AdjustmentItem.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Adjustments/Operations/Create/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Adjustments/Operations/CreateAdjustment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Adjustments/Operations/ListAdjustments.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Adjustments/Operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Adjustments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.640469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Businesses/
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Businesses/BusinessesClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.640469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Businesses/Operations/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Businesses/Operations/CreateBusiness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Businesses/Operations/ListBusinesses.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Businesses/Operations/UpdateBusiness.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Businesses/Operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Businesses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.640469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Customers/
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Customers/CustomersClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.640469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Customers/Operations/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Customers/Operations/CreateCustomer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Customers/Operations/ListCreditBalances.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Customers/Operations/ListCustomers.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Customers/Operations/UpdateCustomer.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Customers/Operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Customers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.640469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Discounts/
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Discounts/DiscountsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.644469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Discounts/Operations/
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Discounts/Operations/CreateDiscount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Discounts/Operations/ListDiscounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Discounts/Operations/UpdateDiscount.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Discounts/Operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Discounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.644469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/EventTypes/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/EventTypes/EventTypesClient.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/EventTypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.644469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Events/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Events/EventsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.644469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Events/Operations/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Events/Operations/ListEvents.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Events/Operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.644469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/NotificationLogs/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/NotificationLogs/NotificationLogsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.644469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/NotificationLogs/Operations/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/NotificationLogs/Operations/ListNotificationLogs.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/NotificationLogs/Operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/NotificationLogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.644469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/NotificationSettings/
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/NotificationSettings/NotificationSettingsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.644469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/NotificationSettings/Operations/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/NotificationSettings/Operations/CreateNotificationSetting.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/NotificationSettings/Operations/UpdateNotificationSetting.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/NotificationSettings/Operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/NotificationSettings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.644469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Notifications/
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Notifications/NotificationsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.644469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Notifications/Operations/
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Notifications/Operations/ListNotifications.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Notifications/Operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.644469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Prices/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.648469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Prices/Operations/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Prices/Operations/CreatePrice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.648469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Prices/Operations/List/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Prices/Operations/List/Includes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Prices/Operations/List/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Prices/Operations/ListPrices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Prices/Operations/UpdatePrice.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Prices/Operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Prices/PricesClient.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.648469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/PricingPreviews/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.648469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/PricingPreviews/Operations/
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/PricingPreviews/Operations/PreviewPrice.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/PricingPreviews/Operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/PricingPreviews/PricingPreviewsClient.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/PricingPreviews/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.648469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Products/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.648469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Products/Operations/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Products/Operations/CreateProduct.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.648469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Products/Operations/List/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Products/Operations/List/Includes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Products/Operations/List/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Products/Operations/ListProducts.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Products/Operations/UpdateProduct.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Products/Operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Products/ProductsClient.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Products/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.648469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Reports/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.648469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Reports/Operations/
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Reports/Operations/CreateReport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Reports/Operations/ListReports.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Reports/Operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Reports/ReportsClient.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.648469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Shared/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.648469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Shared/Operations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.652469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Shared/Operations/List/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Shared/Operations/List/Comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Shared/Operations/List/DateComparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Shared/Operations/List/OrderBy.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Shared/Operations/List/Pager.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Shared/Operations/List/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Shared/Operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Shared/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.652469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.652469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/CancelSubscription.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/CreateOneTimeCharge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.652469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/Get/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/Get/Includes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/Get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/ListSubscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/PauseSubscription.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/PreviewOneTimeCharge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/PreviewUpdateSubscription.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/ResumeSubscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.652469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/Update/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/Update/SubscriptionDiscount.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/Update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/UpdateSubscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/SubscriptionsClient.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.652469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.652469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/Operations/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/Operations/CreateTransaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.656469 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/Operations/List/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/Operations/List/Includes.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/Operations/List/Origin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/Operations/List/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/Operations/ListTransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/Operations/PreviewTransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/Operations/UpdateTransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/Operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/TransactionsClient.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/ResponseParser.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/Undefined.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.664469 paddle-billing-python-sdk-0.1.0b1/paddle_billing_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-02-26 21:07:51.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    29192 2024-02-26 21:07:51.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 21:07:51.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-26 21:07:51.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-26 21:07:51.000000 paddle-billing-python-sdk-0.1.0b1/paddle_billing_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 21:07:51.664469 paddle-billing-python-sdk-0.1.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.656469 paddle-billing-python-sdk-0.1.0b1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.656469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.656469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.656469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Addresses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Addresses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Addresses/test_AddressesClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.656469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Adjustments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Adjustments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Adjustments/test_AdjustmentsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.656469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Businesses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Businesses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Businesses/test_BusinessesClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.656469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Customers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Customers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Customers/test_CustomersClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.656469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Discounts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Discounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Discounts/test_DiscountsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.656469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/EventTypes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/EventTypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/EventTypes/test_EventTypesClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.656469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Events/test_EventsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.656469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/NotificationLogs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/NotificationLogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/NotificationLogs/test_NotificationLogsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.660469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/NotificationSettings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/NotificationSettings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13680 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/NotificationSettings/test_NotificationSettingsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.660469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Notifications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Notifications/test_NotificationsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.660469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Prices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Prices/test_PricesClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.660469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/PricingPreviews/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/PricingPreviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/PricingPreviews/test_PricingPreviewsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.660469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Products/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Products/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Products/test_ProductsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.660469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Reports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Reports/test_ReportsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.660469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35570 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Subscriptions/test_SubscriptionsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.660469 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Transactions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28356 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Transactions/test_TransactionsClient.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.660469 paddle-billing-python-sdk-0.1.0b1/tests/Unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.660469 paddle-billing-python-sdk-0.1.0b1/tests/Unit/Logger/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Unit/Logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Unit/Logger/test_Logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.660469 paddle-billing-python-sdk-0.1.0b1/tests/Unit/Notification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Unit/Notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Unit/Notification/test_Verifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.660469 paddle-billing-python-sdk-0.1.0b1/tests/Unit/PaddleStrEnum/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Unit/PaddleStrEnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Unit/PaddleStrEnum/test_PaddleStrEnum.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:51.664469 paddle-billing-python-sdk-0.1.0b1/tests/Utils/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Utils/FakeResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Utils/ReadsFixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Utils/TestClient.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 21:07:35.000000 paddle-billing-python-sdk-0.1.0b1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.082431 paddle-billing-python-sdk-0.1.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-03-04 22:09:11.082431 paddle-billing-python-sdk-0.1.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5614 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:10.998431 paddle-billing-python-sdk-0.1.0b2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/examples/catalog_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/examples/event_polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/examples/get_products.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/examples/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.002431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/ConditionallyRemoveImportMeta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.006431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Adjustment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.006431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Adjustments/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Adjustments/AdjustmentCustomerBalance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Adjustments/AdjustmentItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Adjustments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Business.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.010431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/AddressCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/AdjustmentCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/BusinessCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/Collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/CreditBalanceCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/CustomerCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/DiscountCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/EventCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/EventTypeCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/NotificationCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/NotificationLogCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/NotificationSettingCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/Paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/PriceCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/ProductCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/ReportCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/SubscriptionCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/SubscriptionPreviewCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/TransactionCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/TransactionPreviewCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/TransactionsDataCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/CreditBalance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/DateTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Discount.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.010431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Discounts/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Discounts/DiscountStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Discounts/DiscountType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Discounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/EventType.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.010431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Events/
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Events/EventTypeName.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/NotificationLog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/NotificationSetting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.010431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/NotificationSettings/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/NotificationSettings/NotificationSettingType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/NotificationSettings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.010431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Notifications/NotificationOrigin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Notifications/NotificationPayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Notifications/NotificationPayoutStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Notifications/NotificationStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/PricePreview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.014431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/PricingPreviews/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/PricingPreviews/PricePreviewDetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/PricingPreviews/PricePreviewDiscounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/PricingPreviews/PricePreviewItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/PricingPreviews/PricePreviewLineItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/PricingPreviews/PricePreviewTotalsFormatted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/PricingPreviews/PricePreviewUnitTotalsFormatted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/PricingPreviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/ReportCSV.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.014431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Reports/ReportFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Reports/ReportFilterName.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Reports/ReportFilterOperator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Reports/ReportStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Reports/ReportType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.022431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/Action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/AddressPreview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/AdjustmentItemTotals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/AdjustmentProration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/AdjustmentStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/AdjustmentTimePeriod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/AdjustmentTotals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/AdjustmentType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/AvailablePaymentMethods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/BillingDetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/BillingDetailsUpdate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/CatalogType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/ChargebackFee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/Checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/CollectionMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/Contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/CountryCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/CurrencyCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/CurrencyCodeAdjustments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/CurrencyCodePayouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/CustomData.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/Data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/ImportMeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/Interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/Meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/MetaPaginated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/MethodDetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/Money.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/Original.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/Pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/PaymentAttemptStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/PaymentMethodType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/PayoutTotalsAdjustment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/PriceQuantity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/Status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TaxCategory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TaxMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TaxRatesUsed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TimePeriod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/Totals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TransactionDetailsPreview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TransactionLineItemPreview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TransactionOrigin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TransactionPaymentAttempt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TransactionPayoutTotals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TransactionPayoutTotalsAdjusted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TransactionStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TransactionTotals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TransactionTotalsAdjusted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/UnitPriceOverride.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/UnitTotals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/SubscriptionPreview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.026431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionAdjustmentItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionAdjustmentPreview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionCharge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionCredit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionDetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionDiscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionEffectiveFrom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionItemStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionItems.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionItemsWithPrice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionManagementUrls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionNextTransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionNonCatalogPrice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionNonCatalogPriceWithProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionNonCatalogProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionOnPaymentFailure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionPreviewSubscriptionUpdateSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionPrice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionProration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionProrationBillingMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionResultAction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionResumeEffectiveFrom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionScheduledChange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionScheduledChangeAction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionTimePeriod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionTransactionItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionTransactionLineItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionUpdateItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/TransactionData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/TransactionPreview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.030431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionAdjustmentsTotals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionBreakdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionCardType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionCreateItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionCreateItemWithPrice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionDetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionItemPreviewWithNonCatalogPrice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionItemPreviewWithPrice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionItemPreviewWithPriceId.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionLineItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionNonCatalogPrice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionNonCatalogPriceWithProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionNonCatalogProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionProration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionTimePeriod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionUpdateTransactionItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/EnumStringify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.030431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/ApiError.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.034431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/ApiErrors/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/ApiErrors/AddressApiError.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/ApiErrors/AdjustmentApiError.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/ApiErrors/BusinessApiError.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/ApiErrors/CustomerApiError.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/ApiErrors/DiscountApiError.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/ApiErrors/PriceApiError.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/ApiErrors/ProductApiError.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/ApiErrors/SubscriptionApiError.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/ApiErrors/TransactionApiError.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/ApiErrors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/FieldError.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/SdkException.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.034431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/SdkExceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/SdkExceptions/InvalidArgumentException.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/SdkExceptions/MalformedResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/SdkExceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/FiltersNone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/FiltersUndefined.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/HasParameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.034431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Logger/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Logger/Formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Logger/NullHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Logger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.034431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.038431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Adjustment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.038431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Adjustments/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Adjustments/AdjustmentItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Adjustments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Business.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.038431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Businesses/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Businesses/BusinessesContacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Businesses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/DateTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Discount.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.038431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Discounts/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Discounts/DiscountStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Discounts/DiscountType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Discounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Payout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.038431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Payouts/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Payouts/PayoutStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Payouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.038431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Reports/ReportFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Reports/ReportFilterName.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Reports/ReportFilterOperator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Reports/ReportStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Reports/ReportType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.046431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/Action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/AddressPreview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/AdjustmentItemTotals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/AdjustmentProration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/AdjustmentStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/AdjustmentTimePeriod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/AdjustmentTotals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/AdjustmentType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/AvailablePaymentMethods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/BillingDetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/Card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/CatalogType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/ChargebackFee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/Checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/CollectionMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/CountryCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/CurrencyCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/CurrencyCodeAdjustments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/CurrencyCodePayouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/CustomData.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/Data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/ImportMeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/Interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/MethodDetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/Money.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/Original.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/PaymentAttemptStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/PaymentMethodType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/PayoutTotalsAdjustment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/PriceQuantity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/Status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/TaxCategory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/TaxMode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/TaxRatesUsed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/TimePeriod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/Totals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/TransactionOrigin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/TransactionPaymentAttempt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/TransactionPayoutTotals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/TransactionPayoutTotalsAdjusted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/TransactionStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/TransactionTotals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/TransactionTotalsAdjusted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/UnitPriceOverride.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/UnitTotals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.050431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionAdjustmentItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionCharge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionCredit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionDiscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionEffectiveFrom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionItemStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionOnPaymentFailure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionPrice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionScheduledChange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionScheduledChangeAction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionStatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionTimePeriod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.050431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transactions/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transactions/TransactionAdjustmentsTotals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transactions/TransactionBreakdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transactions/TransactionCardType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transactions/TransactionDetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transactions/TransactionItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transactions/TransactionLineItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transactions/TransactionProration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transactions/TransactionTimePeriod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.058431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/AddressCreated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/AddressUpdated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/AdjustmentCreated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/AdjustmentUpdated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/BusinessCreated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/BusinessUpdated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/CustomerCreated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/CustomerUpdated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/DiscountCreated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/DiscountImported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/DiscountUpdated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/PayoutCreated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/PayoutPaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/PriceCreated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/PriceUpdated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/ProductCreated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/ProductUpdated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/ReportCreated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/ReportUpdated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/SubscriptionActivated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/SubscriptionCanceled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/SubscriptionCreated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/SubscriptionImported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/SubscriptionPastDue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/SubscriptionPaused.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/SubscriptionResumed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/SubscriptionTrialing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/SubscriptionUpdated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/TransactionBilled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/TransactionCanceled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/TransactionCompleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/TransactionCreated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/TransactionPaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/TransactionPastDue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/TransactionPaymentFailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/TransactionReady.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/TransactionUpdated.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/PaddleSignature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Verifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/PaddleStrEnum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/RecursivelyRemoveKey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.058431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.058431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Addresses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Addresses/AddressesClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.058431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Addresses/Operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Addresses/Operations/CreateAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Addresses/Operations/ListAddresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Addresses/Operations/UpdateAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Addresses/Operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Addresses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.058431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Adjustments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Adjustments/AdjustmentsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.058431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Adjustments/Operations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.058431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Adjustments/Operations/Create/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Adjustments/Operations/Create/AdjustmentItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Adjustments/Operations/Create/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Adjustments/Operations/CreateAdjustment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Adjustments/Operations/ListAdjustments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Adjustments/Operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Adjustments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.058431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Businesses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Businesses/BusinessesClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.062431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Businesses/Operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Businesses/Operations/CreateBusiness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Businesses/Operations/ListBusinesses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Businesses/Operations/UpdateBusiness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Businesses/Operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Businesses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.062431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Customers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Customers/CustomersClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.062431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Customers/Operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Customers/Operations/CreateCustomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Customers/Operations/ListCreditBalances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Customers/Operations/ListCustomers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Customers/Operations/UpdateCustomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Customers/Operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Customers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.062431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Discounts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Discounts/DiscountsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.062431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Discounts/Operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Discounts/Operations/CreateDiscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Discounts/Operations/ListDiscounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Discounts/Operations/UpdateDiscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Discounts/Operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Discounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.062431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/EventTypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/EventTypes/EventTypesClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/EventTypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.062431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Events/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Events/EventsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.062431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Events/Operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Events/Operations/ListEvents.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Events/Operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.062431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/NotificationLogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/NotificationLogs/NotificationLogsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.062431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/NotificationLogs/Operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/NotificationLogs/Operations/ListNotificationLogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/NotificationLogs/Operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/NotificationLogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.066431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/NotificationSettings/
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/NotificationSettings/NotificationSettingsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.066431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/NotificationSettings/Operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/NotificationSettings/Operations/CreateNotificationSetting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/NotificationSettings/Operations/UpdateNotificationSetting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/NotificationSettings/Operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/NotificationSettings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.066431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Notifications/NotificationsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.066431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Notifications/Operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Notifications/Operations/ListNotifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Notifications/Operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.066431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Prices/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.066431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Prices/Operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Prices/Operations/CreatePrice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.066431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Prices/Operations/List/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Prices/Operations/List/Includes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Prices/Operations/List/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Prices/Operations/ListPrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Prices/Operations/UpdatePrice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Prices/Operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Prices/PricesClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.066431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/PricingPreviews/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.066431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/PricingPreviews/Operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/PricingPreviews/Operations/PreviewPrice.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/PricingPreviews/Operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/PricingPreviews/PricingPreviewsClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/PricingPreviews/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.066431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Products/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.070431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Products/Operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Products/Operations/CreateProduct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.070431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Products/Operations/List/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Products/Operations/List/Includes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Products/Operations/List/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Products/Operations/ListProducts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Products/Operations/UpdateProduct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Products/Operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Products/ProductsClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Products/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.070431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Reports/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.070431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Reports/Operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Reports/Operations/CreateReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Reports/Operations/ListReports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Reports/Operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Reports/ReportsClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.070431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Shared/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.070431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Shared/Operations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.070431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Shared/Operations/List/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Shared/Operations/List/Comparator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Shared/Operations/List/DateComparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Shared/Operations/List/OrderBy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Shared/Operations/List/Pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Shared/Operations/List/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Shared/Operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Shared/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.070431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.070431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/CancelSubscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/CreateOneTimeCharge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.074431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/Get/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/Get/Includes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/Get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/ListSubscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/PauseSubscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/PreviewOneTimeCharge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/PreviewUpdateSubscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/ResumeSubscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.074431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/Update/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/Update/SubscriptionDiscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/Update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/UpdateSubscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/SubscriptionsClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.074431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.074431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/Operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/Operations/CreateTransaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.074431 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/Operations/List/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/Operations/List/Includes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/Operations/List/Origin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/Operations/List/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/Operations/ListTransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/Operations/PreviewTransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/Operations/UpdateTransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/Operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/TransactionsClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/ResponseParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/Undefined.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.082431 paddle-billing-python-sdk-0.1.0b2/paddle_billing_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-03-04 22:09:10.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    29192 2024-03-04 22:09:10.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 22:09:10.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-04 22:09:10.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-04 22:09:10.000000 paddle-billing-python-sdk-0.1.0b2/paddle_billing_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 22:09:11.082431 paddle-billing-python-sdk-0.1.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.074431 paddle-billing-python-sdk-0.1.0b2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.074431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.074431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.074431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Addresses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Addresses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Addresses/test_AddressesClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.078431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Adjustments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Adjustments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Adjustments/test_AdjustmentsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.078431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Businesses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Businesses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12772 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Businesses/test_BusinessesClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.078431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Customers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Customers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12629 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Customers/test_CustomersClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.078431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Discounts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Discounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Discounts/test_DiscountsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.078431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/EventTypes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/EventTypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/EventTypes/test_EventTypesClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.078431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Events/test_EventsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.078431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/NotificationLogs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/NotificationLogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/NotificationLogs/test_NotificationLogsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.078431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/NotificationSettings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/NotificationSettings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13680 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/NotificationSettings/test_NotificationSettingsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.078431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9232 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Notifications/test_NotificationsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.078431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Prices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Prices/test_PricesClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.078431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/PricingPreviews/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/PricingPreviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/PricingPreviews/test_PricingPreviewsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.078431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Products/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Products/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Products/test_ProductsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.078431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Reports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Reports/test_ReportsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.082431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35570 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Subscriptions/test_SubscriptionsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.082431 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Transactions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28356 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Transactions/test_TransactionsClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.082431 paddle-billing-python-sdk-0.1.0b2/tests/Unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.082431 paddle-billing-python-sdk-0.1.0b2/tests/Unit/Logger/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Unit/Logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Unit/Logger/test_Logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.082431 paddle-billing-python-sdk-0.1.0b2/tests/Unit/Notification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Unit/Notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Unit/Notification/test_Verifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.082431 paddle-billing-python-sdk-0.1.0b2/tests/Unit/PaddleStrEnum/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Unit/PaddleStrEnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Unit/PaddleStrEnum/test_PaddleStrEnum.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:11.082431 paddle-billing-python-sdk-0.1.0b2/tests/Utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Utils/FakeResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Utils/ReadsFixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Utils/TestClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 22:09:06.000000 paddle-billing-python-sdk-0.1.0b2/tests/__init__.py
```

### Comparing `paddle-billing-python-sdk-0.1.0b1/LICENSE` & `paddle-billing-python-sdk-0.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/PKG-INFO` & `paddle-billing-python-sdk-0.1.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddle-billing-python-sdk
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: A Python wrapper for the Paddle Billing API
 Home-page: https://github.com/invincibear/paddle-billing-python-sdk
 Author: Corey Regan
 Author-email: regan.corey@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.13
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31
 Requires-Dist: urllib3>=1.26.18
 Provides-Extra: dev
-Requires-Dist: pytest~=7.4.4; extra == "dev"
+Requires-Dist: pytest<8.1.0,>=7.4.4; extra == "dev"
 Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
 Requires-Dist: requests-mock~=1.11.0; extra == "dev"
 Requires-Dist: setuptools>=69.0.3; extra == "dev"
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/Invincibear/paddle-billing-python-sdk/publish_to_pypi.yml)](https://github.com/Invincibear/paddle-billing-python-sdk/actions/?query=branch%3Amain)
 [![PyPI](https://img.shields.io/pypi/v/paddle-billing-python-sdk.svg)](https://pypi.python.org/pypi/paddle-billing-python-sdk)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/paddle-billing-python-sdk.svg)](https://pypi.python.org/pypi/paddle-billing-python-sdk/)
@@ -97,15 +97,15 @@
 ``` python
 from paddle_billing import Client
 
 paddle = Client('PADDLE_API_SECRET_KEY')
 
 products = paddle.products.list()
 
-# List() returns an iterable, so pagination is automatically handled
+# list() returns an iterable, so pagination is automatically handled
 for product in products:
     print(f"Product's id: {product.id}")
 ```
 
 ### Get an entity
 You can get an entity with the `get()` method in the resource. It accepts the `id` of the entity to get. The entity is returned.
 ``` python
```

### Comparing `paddle-billing-python-sdk-0.1.0b1/README.md` & `paddle-billing-python-sdk-0.1.0b2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 ``` python
 from paddle_billing import Client
 
 paddle = Client('PADDLE_API_SECRET_KEY')
 
 products = paddle.products.list()
 
-# List() returns an iterable, so pagination is automatically handled
+# list() returns an iterable, so pagination is automatically handled
 for product in products:
     print(f"Product's id: {product.id}")
 ```
 
 ### Get an entity
 You can get an entity with the `get()` method in the resource. It accepts the `id` of the entity to get. The entity is returned.
 ``` python
```

### Comparing `paddle-billing-python-sdk-0.1.0b1/examples/catalog_management.py` & `paddle-billing-python-sdk-0.1.0b2/examples/catalog_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from logging import getLogger
 from os      import getenv
-from sys     import exit  # You should use classes/functions that return instead of exit
+from sys     import exit  # You should use classes/functions that returns instead of exits
 
 from paddle_billing import Client, Environment, Options
 
 from paddle_billing.Entities.Shared import (
     CountryCode,
     CurrencyCode,
     CustomData,
```

### Comparing `paddle-billing-python-sdk-0.1.0b1/examples/event_polling.py` & `paddle-billing-python-sdk-0.1.0b2/examples/event_polling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from logging import getLogger
 from os      import getenv
-from sys     import exit  # You should use classes/functions that return instead of exit
+from sys     import exit  # You should use classes/functions that returns instead of exits
 
 from paddle_billing import Client, Environment, Options
 
 from paddle_billing.Exceptions.ApiError                        import ApiError
 from paddle_billing.Exceptions.SdkExceptions.MalformedResponse import MalformedResponse
 
 from paddle_billing.Resources.Events.Operations import ListEvents
```

### Comparing `paddle-billing-python-sdk-0.1.0b1/examples/get_products.py` & `paddle-billing-python-sdk-0.1.0b2/examples/get_products.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from logging import getLogger
 from os      import getenv
-from sys     import exit  # You should use classes/functions that return instead of exit
+from sys     import exit  # You should use classes/functions that returns instead of exits
 
 from paddle_billing import Client, Environment, Options
 
 from paddle_billing.Exceptions.ApiError                        import ApiError
 from paddle_billing.Exceptions.SdkExceptions.MalformedResponse import MalformedResponse
 
 log = getLogger('my_app')
```

### Comparing `paddle-billing-python-sdk-0.1.0b1/examples/logger.py` & `paddle-billing-python-sdk-0.1.0b2/examples/logger.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Client.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Client.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/ConditionallyRemoveImportMeta.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/ConditionallyRemoveImportMeta.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Address.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Address.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Adjustment.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Adjustment.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Adjustments/AdjustmentItem.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Adjustments/AdjustmentItem.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Business.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Business.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/AddressCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/AddressCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/AdjustmentCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/AdjustmentCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/BusinessCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/BusinessCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/Collection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/Collection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/CreditBalanceCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/CreditBalanceCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/CustomerCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/CustomerCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/DiscountCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/DiscountCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/EventCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/EventCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/EventTypeCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/EventTypeCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/NotificationCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/NotificationCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/NotificationLogCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/NotificationLogCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/NotificationSettingCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/NotificationSettingCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/Paginator.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/Paginator.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/PriceCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/PriceCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/ProductCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/ProductCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/ReportCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/ReportCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/SubscriptionCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/SubscriptionCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/SubscriptionPreviewCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/SubscriptionPreviewCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/TransactionCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/TransactionCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/TransactionPreviewCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/TransactionPreviewCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/TransactionsDataCollection.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/TransactionsDataCollection.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Collections/__init__.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Collections/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/CreditBalance.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/CreditBalance.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Customer.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Customer.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/DateTime.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/DateTime.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Discount.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Discount.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Event.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Event.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/EventType.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/EventType.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Events/EventTypeName.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Events/EventTypeName.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Notification.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Notification.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/NotificationLog.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/NotificationLog.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/NotificationSetting.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/NotificationSetting.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Notifications/NotificationPayout.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Notifications/NotificationPayout.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Price.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Price.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__  import annotations
 from dataclasses import dataclass
+from datetime    import datetime
 
-from paddle_billing.Entities.Entity  import Entity
-
+from paddle_billing.Entities.Entity import Entity
 from paddle_billing.Entities.Shared import (
     CatalogType,
     CustomData,
     ImportMeta,
     Money,
     PriceQuantity,
     Status,
@@ -32,27 +32,31 @@
     unit_price:           Money
     unit_price_overrides: list[UnitPriceOverride]
     quantity:             PriceQuantity
     status:               Status
     custom_data:          CustomData | None
     import_meta:          ImportMeta | None
     product:              Product    | None
+    created_at:           datetime
+    updated_at:           datetime
 
 
     @classmethod
     def from_dict(cls, data: dict) -> Price:
         return Price(
             id                   = data['id'],
             product_id           = data['product_id'],
             name                 = data.get('name'),
             description          = data['description'],
             unit_price           = Money.from_dict(data['unit_price']),
             quantity             = PriceQuantity.from_dict(data['quantity']),
             status               = Status(data['status']),
             tax_mode             = TaxMode(data.get('tax_mode')),
+            created_at           = datetime.fromisoformat(data['created_at']),
+            updated_at           = datetime.fromisoformat(data['updated_at']),
             unit_price_overrides = [UnitPriceOverride.from_dict(override) for override in data.get('unit_price_overrides', [])],
             type                 = CatalogType(data.get('type'))               if data.get('type')          else None,
             billing_cycle        = TimePeriod.from_dict(data['billing_cycle']) if data.get('billing_cycle') else None,
             trial_period         = TimePeriod.from_dict(data['trial_period'])  if data.get('trial_period')  else None,
             custom_data          = CustomData(data['custom_data'])             if data.get('custom_data')   else None,
             import_meta          = ImportMeta.from_dict(data['import_meta'])   if data.get('import_meta')   else None,
             product              = Product.from_dict(data['product'])          if data.get('product')       else None,
```

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/PricePreview.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/PricePreview.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/PricingPreviews/PricePreviewDiscounts.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/PricingPreviews/PricePreviewDiscounts.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/PricingPreviews/PricePreviewLineItem.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/PricingPreviews/PricePreviewLineItem.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/PricingPreviews/__init__.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/PricingPreviews/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Product.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Product.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 from __future__  import annotations
 from dataclasses import dataclass
 from datetime    import datetime
 
-from paddle_billing.Entities.Entity import Entity
-from paddle_billing.Entities.Shared import CatalogType, CustomData, ImportMeta, Status, TaxCategory
+from paddle_billing.Notifications.Entities.Entity import Entity
+from paddle_billing.Notifications.Entities.Shared import CatalogType, CustomData, ImportMeta, Status, TaxCategory
 
 
 @dataclass
 class Product(Entity):
     id:           str
     name:         str
     status:       Status
     tax_category: TaxCategory
     description:  str         | None
     image_url:    str         | None
-    created_at:   datetime    | None = None
     custom_data:  CustomData  | None = None
     import_meta:  ImportMeta  | None = None
     prices:       list[Price] | None = None
     type:         CatalogType | None = None
+    created_at:   datetime    | None = None
+    updated_at:   datetime    | None = None
 
 
     @classmethod
     def from_dict(cls, data: dict) -> Product:
         return Product(
             description  = data.get('description'),
             id           = data['id'],
             image_url    = data.get('image_url'),
             name         = data['name'],
             status       = Status(data['status']),
             tax_category = TaxCategory(data['tax_category']),
             prices       = [Price.from_dict(price) for price in data.get('prices', [])],
             type         = CatalogType(data['type'])                  if data.get('type')        else None,
             custom_data  = CustomData(data['custom_data'])            if data.get('custom_data') else None,
-            created_at   = datetime.fromisoformat(data['created_at']) if data.get('created_at')  else None,
             import_meta  = ImportMeta.from_dict(data['import_meta'])  if data.get('import_meta') else None,
+            created_at   = datetime.fromisoformat(data['created_at']) if data.get('created_at')  else None,
+            updated_at   = datetime.fromisoformat(data['updated_at']) if data.get('updated_at')  else None,
         )
 
 
 
 # Prevents circular import
 from paddle_billing.Entities.Price  import Price  # noqa E402
```

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Report.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Report.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/AdjustmentTotals.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/AdjustmentTotals.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/BillingDetails.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/BillingDetails.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/BillingDetailsUpdate.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/BillingDetailsUpdate.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/Card.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/Card.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/CountryCode.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/CountryCode.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/CurrencyCode.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/CurrencyCode.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/ErrorCode.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/MethodDetails.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/MethodDetails.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/Money.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/Money.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/PayoutTotalsAdjustment.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/PayoutTotalsAdjustment.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TaxCategory.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TaxCategory.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TransactionDetailsPreview.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TransactionDetailsPreview.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TransactionLineItemPreview.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TransactionLineItemPreview.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TransactionPaymentAttempt.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TransactionPaymentAttempt.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TransactionPayoutTotals.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TransactionPayoutTotals.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TransactionPayoutTotalsAdjusted.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TransactionPayoutTotalsAdjusted.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TransactionTotals.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TransactionTotals.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/TransactionTotalsAdjusted.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/TransactionTotalsAdjusted.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/UnitPriceOverride.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/UnitPriceOverride.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Shared/__init__.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Shared/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscription.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscription.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/SubscriptionPreview.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/SubscriptionPreview.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionAdjustmentItem.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionAdjustmentItem.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionAdjustmentPreview.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionAdjustmentPreview.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionDetails.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionDetails.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionDiscount.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionDiscount.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionItem.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionItem.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionItemsWithPrice.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionItemsWithPrice.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionNextTransaction.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionNextTransaction.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionNonCatalogPrice.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionNonCatalogPrice.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionNonCatalogPriceWithProduct.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionNonCatalogPriceWithProduct.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionNonCatalogProduct.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionNonCatalogProduct.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionPreviewSubscriptionUpdateSummary.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionPreviewSubscriptionUpdateSummary.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionPrice.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionPrice.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionProration.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionProration.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionResult.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionResult.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionScheduledChange.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionScheduledChange.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionTransactionItem.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionTransactionItem.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/SubscriptionTransactionLineItem.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/SubscriptionTransactionLineItem.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Subscriptions/__init__.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Subscriptions/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transaction.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transaction.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/TransactionPreview.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/TransactionPreview.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionAdjustmentsTotals.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionAdjustmentsTotals.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionDetails.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionDetails.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionItem.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionItem.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionItemPreviewWithNonCatalogPrice.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionItemPreviewWithNonCatalogPrice.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionItemPreviewWithPrice.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionItemPreviewWithPrice.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionItemPreviewWithPriceId.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionItemPreviewWithPriceId.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionLineItem.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionLineItem.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionNonCatalogPrice.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionNonCatalogPrice.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionNonCatalogPriceWithProduct.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionNonCatalogPriceWithProduct.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionNonCatalogProduct.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionNonCatalogProduct.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/TransactionProration.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/TransactionProration.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Entities/Transactions/__init__.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Exceptions/ApiError.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Exceptions/ApiError.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Logger/Formatter.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Logger/Formatter.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Logger/__init__.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Logger/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Address.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Address.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Adjustment.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Adjustment.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Adjustments/AdjustmentItem.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Adjustments/AdjustmentItem.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Business.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Business.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Customer.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Customer.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/DateTime.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/DateTime.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Discount.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Discount.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Payout.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Payout.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Price.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Price.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__  import annotations
 from dataclasses import dataclass
+from datetime    import datetime
 
 from paddle_billing.Notifications.Entities.Entity import Entity
 from paddle_billing.Notifications.Entities.Shared import (
     CatalogType,
     CustomData,
     ImportMeta,
     Money,
@@ -30,15 +31,16 @@
     tax_mode:             TaxMode
     unit_price:           Money
     unit_price_overrides: list[UnitPriceOverride]
     quantity:             PriceQuantity
     status:               Status
     custom_data:          CustomData | None
     import_meta:          ImportMeta | None
-    # product:              Product    | None
+    created_at:           datetime   | None
+    updated_at:           datetime   | None
 
 
     @classmethod
     def from_dict(cls, data: dict) -> Price:
         return Price(
             id                   = data['id'],
             product_id           = data['product_id'],
@@ -50,14 +52,15 @@
             tax_mode             = TaxMode(data.get('tax_mode')),
             unit_price_overrides = [UnitPriceOverride.from_dict(override) for override in data.get('unit_price_overrides', [])],
             type                 = CatalogType(data.get('type'))               if data.get('type')          else None,
             billing_cycle        = TimePeriod.from_dict(data['billing_cycle']) if data.get('billing_cycle') else None,
             trial_period         = TimePeriod.from_dict(data['trial_period'])  if data.get('trial_period')  else None,
             custom_data          = CustomData(data['custom_data'])             if data.get('custom_data')   else None,
             import_meta          = ImportMeta.from_dict(data['import_meta'])   if data.get('import_meta')   else None,
-            # product              = Product.from_dict(data['product'])          if data.get('product')       else None,
+            created_at           = datetime.fromisoformat(data['created_at'])  if data.get('created_at')    else None,
+            updated_at           = datetime.fromisoformat(data['updated_at'])  if data.get('updated_at')    else None,
         )
 
 
 
 # Prevents circular import
 from paddle_billing.Entities.Product import Product  # noqa E402
```

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Product.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Entities/Product.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from __future__  import annotations
 from dataclasses import dataclass
 from datetime    import datetime
 
-from paddle_billing.Notifications.Entities.Entity import Entity
-from paddle_billing.Notifications.Entities.Shared import CatalogType, CustomData, ImportMeta, Status, TaxCategory
+from paddle_billing.Entities.Entity import Entity
+from paddle_billing.Entities.Shared import CatalogType, CustomData, ImportMeta, Status, TaxCategory
 
 
 @dataclass
 class Product(Entity):
     id:           str
     name:         str
     status:       Status
     tax_category: TaxCategory
+    created_at:   datetime
+    updated_at:   datetime
     description:  str         | None
     image_url:    str         | None
-    created_at:   datetime    | None = None
     custom_data:  CustomData  | None = None
     import_meta:  ImportMeta  | None = None
     prices:       list[Price] | None = None
     type:         CatalogType | None = None
 
 
     @classmethod
@@ -26,18 +27,19 @@
         return Product(
             description  = data.get('description'),
             id           = data['id'],
             image_url    = data.get('image_url'),
             name         = data['name'],
             status       = Status(data['status']),
             tax_category = TaxCategory(data['tax_category']),
+            created_at   = datetime.fromisoformat(data['created_at']),
+            updated_at   = datetime.fromisoformat(data['updated_at']),
             prices       = [Price.from_dict(price) for price in data.get('prices', [])],
             type         = CatalogType(data['type'])                  if data.get('type')        else None,
             custom_data  = CustomData(data['custom_data'])            if data.get('custom_data') else None,
-            created_at   = datetime.fromisoformat(data['created_at']) if data.get('created_at')  else None,
             import_meta  = ImportMeta.from_dict(data['import_meta'])  if data.get('import_meta') else None,
         )
 
 
 
 # Prevents circular import
 from paddle_billing.Entities.Price  import Price  # noqa E402
```

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Report.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Report.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/AdjustmentProration.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/AdjustmentProration.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/AdjustmentTotals.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/AdjustmentTotals.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/BillingDetails.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/BillingDetails.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/Card.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/Card.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/CountryCode.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/CountryCode.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/CurrencyCode.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/CurrencyCode.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/ErrorCode.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/MethodDetails.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/MethodDetails.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/Money.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/Money.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/PayoutTotalsAdjustment.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/PayoutTotalsAdjustment.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/TaxCategory.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/TaxCategory.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/TransactionPaymentAttempt.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/TransactionPaymentAttempt.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/TransactionPayoutTotals.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/TransactionPayoutTotals.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/TransactionPayoutTotalsAdjusted.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/TransactionPayoutTotalsAdjusted.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/TransactionTotals.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/TransactionTotals.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/TransactionTotalsAdjusted.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/TransactionTotalsAdjusted.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/UnitPriceOverride.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/UnitPriceOverride.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Shared/__init__.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Shared/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscription.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscription.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionAdjustmentItem.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionAdjustmentItem.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionDiscount.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionDiscount.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionItem.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionItem.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionPrice.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionPrice.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionScheduledChange.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/SubscriptionScheduledChange.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Subscriptions/__init__.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Subscriptions/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transaction.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transaction.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transactions/TransactionAdjustmentsTotals.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transactions/TransactionAdjustmentsTotals.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transactions/TransactionDetails.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transactions/TransactionDetails.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transactions/TransactionItem.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transactions/TransactionItem.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transactions/TransactionLineItem.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transactions/TransactionLineItem.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transactions/TransactionProration.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transactions/TransactionProration.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Entities/Transactions/__init__.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Entities/Transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/PaddleSignature.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/PaddleSignature.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Notifications/Verifier.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Notifications/Verifier.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/PaddleStrEnum.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/PaddleStrEnum.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Addresses/AddressesClient.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Addresses/AddressesClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Addresses/Operations/CreateAddress.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Addresses/Operations/CreateAddress.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Addresses/Operations/ListAddresses.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Addresses/Operations/ListAddresses.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Addresses/Operations/UpdateAddress.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Addresses/Operations/UpdateAddress.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Adjustments/AdjustmentsClient.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Adjustments/AdjustmentsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Adjustments/Operations/CreateAdjustment.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Adjustments/Operations/CreateAdjustment.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Adjustments/Operations/ListAdjustments.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Adjustments/Operations/ListAdjustments.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Businesses/BusinessesClient.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Businesses/BusinessesClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Businesses/Operations/CreateBusiness.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Businesses/Operations/CreateBusiness.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Businesses/Operations/ListBusinesses.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Businesses/Operations/ListBusinesses.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Businesses/Operations/UpdateBusiness.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Businesses/Operations/UpdateBusiness.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Customers/CustomersClient.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Customers/CustomersClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Customers/Operations/ListCreditBalances.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Customers/Operations/ListCreditBalances.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Customers/Operations/ListCustomers.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Customers/Operations/ListCustomers.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Customers/Operations/UpdateCustomer.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Customers/Operations/UpdateCustomer.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Discounts/DiscountsClient.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Discounts/DiscountsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Discounts/Operations/CreateDiscount.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Discounts/Operations/CreateDiscount.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Discounts/Operations/ListDiscounts.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Discounts/Operations/ListDiscounts.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Discounts/Operations/UpdateDiscount.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Discounts/Operations/UpdateDiscount.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/EventTypes/EventTypesClient.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/EventTypes/EventTypesClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Events/EventsClient.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Events/EventsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/NotificationLogs/NotificationLogsClient.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/NotificationLogs/NotificationLogsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/NotificationSettings/NotificationSettingsClient.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/NotificationSettings/NotificationSettingsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/NotificationSettings/Operations/CreateNotificationSetting.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/NotificationSettings/Operations/CreateNotificationSetting.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/NotificationSettings/Operations/UpdateNotificationSetting.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/NotificationSettings/Operations/UpdateNotificationSetting.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Notifications/NotificationsClient.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Notifications/NotificationsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Notifications/Operations/ListNotifications.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Notifications/Operations/ListNotifications.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Prices/Operations/CreatePrice.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Prices/Operations/CreatePrice.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Prices/Operations/ListPrices.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Prices/Operations/ListPrices.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Prices/Operations/UpdatePrice.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Prices/Operations/UpdatePrice.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Prices/PricesClient.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Prices/PricesClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/PricingPreviews/Operations/PreviewPrice.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/PricingPreviews/Operations/PreviewPrice.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/PricingPreviews/PricingPreviewsClient.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/PricingPreviews/PricingPreviewsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Products/Operations/CreateProduct.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Products/Operations/CreateProduct.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Products/Operations/ListProducts.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Products/Operations/ListProducts.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Products/Operations/UpdateProduct.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Products/Operations/UpdateProduct.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Products/ProductsClient.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Products/ProductsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Reports/Operations/CreateReport.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Reports/Operations/CreateReport.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Reports/Operations/ListReports.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Reports/Operations/ListReports.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Reports/ReportsClient.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Reports/ReportsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Shared/Operations/List/DateComparison.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Shared/Operations/List/DateComparison.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Shared/Operations/List/Pager.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Shared/Operations/List/Pager.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/CreateOneTimeCharge.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/CreateOneTimeCharge.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/ListSubscriptions.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/ListSubscriptions.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/PauseSubscription.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/PauseSubscription.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/PreviewOneTimeCharge.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/PreviewOneTimeCharge.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/PreviewUpdateSubscription.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/PreviewUpdateSubscription.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/ResumeSubscription.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/ResumeSubscription.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/UpdateSubscription.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/UpdateSubscription.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/Operations/__init__.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/Operations/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Subscriptions/SubscriptionsClient.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Subscriptions/SubscriptionsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/Operations/CreateTransaction.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/Operations/CreateTransaction.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/Operations/ListTransactions.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/Operations/ListTransactions.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/Operations/PreviewTransaction.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/Operations/PreviewTransaction.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/Operations/UpdateTransaction.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/Operations/UpdateTransaction.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/Operations/__init__.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/Operations/__init__.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/Resources/Transactions/TransactionsClient.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/Resources/Transactions/TransactionsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing/ResponseParser.py` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing/ResponseParser.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing_python_sdk.egg-info/PKG-INFO` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing_python_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddle-billing-python-sdk
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: A Python wrapper for the Paddle Billing API
 Home-page: https://github.com/invincibear/paddle-billing-python-sdk
 Author: Corey Regan
 Author-email: regan.corey@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.13
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31
 Requires-Dist: urllib3>=1.26.18
 Provides-Extra: dev
-Requires-Dist: pytest~=7.4.4; extra == "dev"
+Requires-Dist: pytest<8.1.0,>=7.4.4; extra == "dev"
 Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
 Requires-Dist: requests-mock~=1.11.0; extra == "dev"
 Requires-Dist: setuptools>=69.0.3; extra == "dev"
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/Invincibear/paddle-billing-python-sdk/publish_to_pypi.yml)](https://github.com/Invincibear/paddle-billing-python-sdk/actions/?query=branch%3Amain)
 [![PyPI](https://img.shields.io/pypi/v/paddle-billing-python-sdk.svg)](https://pypi.python.org/pypi/paddle-billing-python-sdk)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/paddle-billing-python-sdk.svg)](https://pypi.python.org/pypi/paddle-billing-python-sdk/)
@@ -97,15 +97,15 @@
 ``` python
 from paddle_billing import Client
 
 paddle = Client('PADDLE_API_SECRET_KEY')
 
 products = paddle.products.list()
 
-# List() returns an iterable, so pagination is automatically handled
+# list() returns an iterable, so pagination is automatically handled
 for product in products:
     print(f"Product's id: {product.id}")
 ```
 
 ### Get an entity
 You can get an entity with the `get()` method in the resource. It accepts the `id` of the entity to get. The entity is returned.
 ``` python
```

### Comparing `paddle-billing-python-sdk-0.1.0b1/paddle_billing_python_sdk.egg-info/SOURCES.txt` & `paddle-billing-python-sdk-0.1.0b2/paddle_billing_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/setup.py` & `paddle-billing-python-sdk-0.1.0b2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools  import setup, find_packages
 
 
 setup(
-    version          = '0.1.0b1',
+    version          = '0.1.0b2',
 
     author           = 'Corey Regan',
     author_email     = 'regan.corey@gmail.com',
     description      = 'A Python wrapper for the Paddle Billing API',
     name             = 'paddle-billing-python-sdk',
     packages         = find_packages(),
     python_requires  = '>=3.11',
@@ -22,15 +22,15 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: 3.13',
     ],
     extras_require = {
         'dev': [
-            'pytest~=7.4.4',
+            'pytest>=7.4.4,<8.1.0',
             'pytest-cov~=4.1.0',
             'requests-mock~=1.11.0',
             'setuptools>=69.0.3',
         ],
     },
     install_requires = [
         'requests>=2.31',
```

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Addresses/test_AddressesClient.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Addresses/test_AddressesClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Adjustments/test_AdjustmentsClient.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Adjustments/test_AdjustmentsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Businesses/test_BusinessesClient.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Businesses/test_BusinessesClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Customers/test_CustomersClient.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Customers/test_CustomersClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Discounts/test_DiscountsClient.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Discounts/test_DiscountsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/EventTypes/test_EventTypesClient.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/EventTypes/test_EventTypesClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Events/test_EventsClient.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Events/test_EventsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/NotificationLogs/test_NotificationLogsClient.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/NotificationLogs/test_NotificationLogsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/NotificationSettings/test_NotificationSettingsClient.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/NotificationSettings/test_NotificationSettingsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Notifications/test_NotificationsClient.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Notifications/test_NotificationsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Prices/test_PricesClient.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Prices/test_PricesClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/PricingPreviews/test_PricingPreviewsClient.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/PricingPreviews/test_PricingPreviewsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Products/test_ProductsClient.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Products/test_ProductsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Reports/test_ReportsClient.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Reports/test_ReportsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Subscriptions/test_SubscriptionsClient.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Subscriptions/test_SubscriptionsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Functional/Resources/Transactions/test_TransactionsClient.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Functional/Resources/Transactions/test_TransactionsClient.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Unit/Notification/test_Verifier.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Unit/Notification/test_Verifier.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Unit/PaddleStrEnum/test_PaddleStrEnum.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Unit/PaddleStrEnum/test_PaddleStrEnum.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Utils/ReadsFixture.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Utils/ReadsFixture.py`

 * *Files identical despite different names*

### Comparing `paddle-billing-python-sdk-0.1.0b1/tests/Utils/TestClient.py` & `paddle-billing-python-sdk-0.1.0b2/tests/Utils/TestClient.py`

 * *Files identical despite different names*
