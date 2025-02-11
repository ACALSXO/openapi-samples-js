# OpenAPI JavaScript Sample Repository

This repository contains sample files demonstrating OpenAPI interactions in JavaScript that can be run in the browser. Each of the included samples is designed as standalone HTML with vanilla JS and no dependecies.

To try these samples yourself, download/clone this repo and load the HTML files locally, or navigate to [this interactive page](https://saxobank.github.io/openapi-samples-js/) to run the samples directly online.

## Requirements

Samples run against Saxo's simulation environment and require an **access token** in order to function. Saxo provides 24-hour tokens on the [Developer Portal](https://www.developer.saxo/openapi/token/), which is the easiest way to get started with the samples provided here. An account is required to generate a token, which can be created for free.

## Table of Contents

1. Authentication
   - [OAuth2 Code Flow example](authentication/oauth2-code-flow)
   - [OAuth2 Implicit Flow example](authentication/oauth2-implicit-flow)
   - [OAuth2 PKCE Flow example](authentication/oauth2-pkce-flow)
   - [Claims in Jwt Token](authentication/token-explained/)
2. Basics
   - [Get user info](basics/user-info)
   - [Query options $top, $skip and \_\_next](basics/query-options)
   - [Error handling](error-handling)
   - [Diagnostics and method override](basics/diagnostics)
3. Instruments
   - [Instrument Search example](instruments/instrument-search)
   - [Extended AssetTypes](instruments/extended-assettypes)
   - [Retrieve Universe](instruments/instrument-retrieval)
4. Order Placement
   - [Basic Order example (stocks, bonds, etf, etc.)](orders/stocks)
   - [Option Order](orders/options)
   - [Option Strategy Order](orders/option-strategies)
   - [Future Order](orders/futures)
   - [OCO Order](orders/oco-orders)
   - [Algorithmic Order](orders/algo-orders)
   - [Conditional Order](orders/conditional-orders)
   - [Regulatory requirements for order tickets](orders/regulatory-requirements)
5. Portfolio
   - [Display Positions and Order List](portfolio/positions-orders)
   - [Netting (RealTime vs EndOfDay)](portfolio/netting)
   - [Margin calculation](portfolio/margin)
   - [Account statements and Export (PDF, Excel)](portfolio/download-reports)
6. Using websockets
   - [Retrieving Order Events](websockets/order-events-monitoring)
   - [Monitoring Primary Status](websockets/primary-monitoring)
   - [Realtime Quotes and Protocol Buffers](websockets/realtime-quotes)
   - [Trade Messages](websockets/trade-messages)
   - [Historical Market Data](websockets/historical-market-data)
   - [Options chain](websockets/options-chain)
7. Batch Requests
   - [Batch Request example](batch-request)

## Sample Apps

[Basic Price Streamer](sample-apps/realtime-quotes/): Shows how to display prices for instruments and update them when an update is broadcasted. The connection health is monitored.

[Basic Order Manager](sample-apps/basic-order-manager/): A Vue.js app that runs in the browser, pulls out open orders of the logged-in client and displays them in a Vuetify table with sorting and filtering functionality. Includes a simple order blotter and an implementation of OAuth implicit flow to authenticate with the OpenAPI.

Suggestions? Comments? Reach us via Github or openapisupport@saxobank.com
