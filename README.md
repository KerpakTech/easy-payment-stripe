# easy-payment-stripe

KerpakTech fork of the Stripe adaptor for [easy-payment](https://github.com/KerpakTech/easy-payment-main).

## Installation

```bash
npm install -save easy-payment @easy-payment/stripe
```

## Usage

```javascript
import Gateways from 'easy-payment';
import Stripe from '@easy-payment/stripe';

const settings = {
  SECRET_KEY: 'SECRET_KEY',
};
const client = Gateways.create(Stripe.gateway, settings);
```

## Gateway API

Implements the [BaseGateway](https://github.com/KerpakTech/easy-payment-base) API plus Stripe Connect helpers used by Kerpak (`createPayment`, `capturePayment`, `cancelPayment`, `updatePayment`, …).
