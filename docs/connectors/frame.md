# `web3-react` Documentation - Frame

- [Install](#install)
- [Arguments](#arguments)
- [Example](#example)
- [Errors](#errors)
  - [UserRejectedRequestError](#userrejectedrequesterror)
    - [Example](#example-1)

## Install
`yarn add @web3-double-react/frame-connector`

## Arguments
```typescript
supportedChainIds: number[]
```

## Example
```javascript
import { FrameConnector } from '@web3-double-react/frame-connector'

const frame = new FrameConnector({ supportedChainIds: [1] })
```

## Errors

### UserRejectedRequestError

#### Example
```javascript
import { UserRejectedRequestError } from '@web3-double-react/frame-connector'

function Component () {
  const { error } = useWeb3React()
  const isUserRejectedRequestError = error instanceof UserRejectedRequestError
  // ...
}
```
