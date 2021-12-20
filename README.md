# proposal-permission-api-based-User-Defined-Isolated-Spaces
Create a Shared Context between Others Context Scopes even Cross Origin first implementation sharedRaw Memory

## Pollyfill
a context (at present only url scope is possible so origin)

- https://developer.chrome.com/blog/enabling-shared-array-buffer/#origin-trial
- https://web.dev/cross-origin-isolation-guide/

The idea is to pass such a cross origin isolated context to existing contexts via a pks (pre known secret) like contextId to enable cross context communication via for example 

## Use cases (Browser)
- a sharedArray Buffer that gets used by 2 wasm modules running on diffrent origins
  - allows cross origin in memory communication without serialization conversation overhead.

## Dream use case (Desktop Apps)
a Chrome Extension or App could maybe get raw pointer memory access to allow full process interop with any application on the device.
