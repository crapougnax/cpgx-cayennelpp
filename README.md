# Cayenne LPP

A Node module to encode and decode Cayenne Low Power Payload for LoraWan

## Usage

```javascript

import { LPPEncoder,LPPDecoder } from  '@crapougnax/cayennelpp'

const encoder = new LPPEncoder()
encoder.addTemperature(99, 33.0)
const pl = encoder.getPayload().toString('base64')

const decoder = new LPPEncoder(buffer)
decoder.decode()
const temperature1 = decoder.getChannel(1).temperature
```

## Test

```bash
npm test
```
