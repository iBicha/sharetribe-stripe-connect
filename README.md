# Sharetribe integrated with Stripe Connect

Sharetribe allows you to create an online marketplace in an instant.

Stripe Connect allows you to create accounts on behalf of your customers so that they can take payments for the items they post on you marketplace, and you can take a fee from each transaction.

This implementation utilises Stripe Connect's ['standalone'](https://stripe.com/docs/connect/standalone-accounts) accounts.  'Managed' accounts allow you more control over the Stripe dashboard and your customers' interactions with Stripe.  But this is a basic implementation.

## Getting Started

This library is a fork of [Sharetribe](https://github.com/sharetribe/sharetribe)

I will be maintaining this library for the minute as I am working on a client application and want to continue to open source the project.

Please follow Sharetribe's installation instructions, using the code from this fork.

## After installation

Once you setup your marketplace, you can head into the admin area and enter details for your Stripe Connect account which can be found in your [Stripe Dashboard](https://dashboard.stripe.com/test/dashboard) under 'your account'. Stripe account setup is fairly easy and you can skip adding bank account details if you like.

Ensure for your local development environment or while testing on a hosted site to switch your Stripe account to 'TEST' and use the test keys.

With Stripe connected via your marketplace's account, sellers in your marketplace can now go into their account and choose 'payment settings', where they can click to connect their Stripe Account (or, more likely, setup a new Stripe Account and connect it).  

At this point, if the user has listings posted, the warnings about needing to setup Stripe should disappear, and they will be able to take payments.

## Deploying to Heroku

See [instructions here](https://github.com/jarvisjohnson/sharetribe-stripe-connect/blob/master/heroku-deploy-gist/Deploying%20Sharetribe%20to%20Heroku.md)
