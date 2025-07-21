# Worldpay Text-to-Pay API

This repository contains the Worldpay Text-to-Pay Collection and environment template for the Worldpay Text-to-Pay API. This collection allows you to quickly get started with integrating payment requests via SMS to your customers.

## Overview

The Text-to-Pay API allows merchants to:
- Manage merchant settings
- Create and manage customers
- Send payment requests via SMS
- Track payment status

## Getting Started

### Prerequisites

1. [Postman](https://www.postman.com/downloads/) installed on your machine
2. Worldpay API Key
3. Worldpay Merchant ID (MID)

### Installation

1. Clone this repository or download the ZIP file
   ```
   git clone https://github.com/your-username/worldpay-text-to-pay-api.git
   ```

2. Open Postman and click on **Import** in the top left corner

3. Upload or drag both files into the import dialog:
   - `text-to-pay.postman_collection.json`
   - `text-to-pay-environment.json`

### Setting Up Your Environment

1. In Postman, select the **Environments** tab from the left sidebar
2. Click on the **Worldpay Text-to-Pay Environment** that you just imported
3. Fill in your specific values:
   - `API_BASE_URL`: Default is `https://apis.stage.worldpay.com/text-to-pay` (change to production URL when ready)
   - `WORLDPAY_API_KEY`: Your Worldpay API key
   - `WORLDPAY_MID`: Your Worldpay Merchant ID
   - `CUSTOMER_PHONE`: Must be set to your phone number (ex: +11232222222)
4. Click **Save**

## Using the Collection

The collection is organized into three main folders:

### 1. Merchant Settings
- Get your merchant profile
- Update merchant settings like logos, colors, and contact information

### 2. Manage Customers
- Create customers with phone numbers for SMS communication
- Update, retrieve, or delete customer information

### 3. Payments
- Create payment requests that will be sent to customers via SMS
- Monitor payment status

### Workflow Example

1. Verify your credentials with **Get Merchant**
2. Create a customer using **Create Customer**
3. Send a payment request using **Create Payment**

## Environment Variables

| Variable | Description | Default Value |
|----------|-------------|---------------|
| API_BASE_URL | Base URL for the API | https://apis.stage.worldpay.com/text-to-pay |
| WORLDPAY_API_KEY | Your API key | (must be set) |
| WORLDPAY_MID | Your merchant ID | (must be set) |
| CUSTOMER_PHONE | Phone number for test customer | (must be set to your phone number ex: +11232222222) |
| CUSTOMER_ID | ID of created customer | (set automatically) |

## Documentation

For detailed information about each endpoint, refer to the official [Worldpay Developer Documentation](https://docs.worldpay.com).

## Support

If you encounter any issues or have questions, please:
1. Open an issue in this repository
2. Contact Worldpay technical support at [techsupport@worldpay.com](mailto:techsupport@worldpay.com)

## License

This project is licensed under the MIT License - see the LICENSE file for details.