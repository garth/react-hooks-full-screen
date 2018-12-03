# react-hooks-full-screen

A react hooks approach to the Fullscreen API.

> Disclaimer: To use hooks a pre-release version of react 16.7 is required. Since the hooks API is subject to change, this library may or may not work with future versions of react.

## Install

```
yarn add react-hooks-full-screen
```

or

```
npm install react-hooks-full-screen
```

## Usage Example

```tsx
import React, { useState } from 'react'
import { useFullScreen } from 'react-hooks-full-screen'

const App: React.StatelessComponent = () => {
  const [showFullScreen, setShowFullScreen] = useState(false)
  useFullScreen('app', showFullScreen)

  return (
    <div id="app">
      <button onClick={() => setShowFullScreen(!showFullScreen)}>Toggle</button>
    </div>
  )
}

export default App
```
