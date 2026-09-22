# resin-api

Official TypeScript type definitions and API contract for **Resin** plugins.

## Installation

```bash
npm install -D resin-api
```

## Quick Start

```typescript
import { Plugin } from "resin-api";

export default class MyPlugin extends Plugin {
  async onLoad() {
    this.addRibbonIcon("SparkleIcon", "My Plugin", () => {
      console.log("Clicked ribbon!");
    });
  }

  async onUnload() {
    console.log("Unloading plugin...");
  }
}
```

