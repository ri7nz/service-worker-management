# SW-Management.

PWA - Service Worker Management

## Usage

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

#### Table of Contents

- [SWRegister](#swregister)
    -   [Examples](#examples)

### SWRegister

An Example how to use SW-management.

#### Examples

```javascript
// src/index.js
import SWRegister from 'sw-management'

// Registration of Service - Worker
const swURL = 'https://example.com/service-worker.js' 
SWRegister.register(
 swURL,
 {
   onRegister: () => console.log('Has Registered with:', swURL)
 }
)

// Checking all of service-worker registered by SW-Management
SWRegister.all()

// Unregister All Service Worker
SWRegister.unregister()
```
