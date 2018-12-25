# Fresh UI

## Based on Mint UI

> Mobile UI elements for **Vue 3.0**

## Installation
```shell
npm i fresh-ui -S
```

## Usage

Import all components.

```javascript
import Vue from 'vue';
import Fresh from 'fresh-ui';
import 'fresh-ui/lib/style.css';

Vue.use(Fresh);
```

Or import specified component. (Use [babel-plugin-component](https://www.npmjs.com/package/babel-plugin-component))

```javascript
import { Cell, Checklist } from 'fresh-ui';

Vue.component(Cell.name, Cell);
Vue.component(Checklist.name, Checklist);
```


Equals to

```javascript
import Vue from 'vue';
import Fresh from 'fresh-ui';
import 'fresh-ui/lib/style.css';

Vue.use(Fresh);

// import specified component

import MtRadio from 'fresh-ui/lib/radio';
import 'fresh-ui/lib/radio/style.css';

Vue.component(MtRadio.name, MtRadio);
```

## babel-plugin-component
- Auto import css file
- Modular import component

Installation
```shell
npm i babel-plugin-component -D
```

Usage

.babelrc
```json
{
  "plugins": ["other-plugin", ["component", [
    { "libraryName": "fresh-ui", "style": true }
  ]]]
}
```

## Development

```shell
npm run dev
```

## Contribution
Please make sure to read the [Contributing Guide](https://github.com/crazywolf132/fresh-ui/blob/master/.github/CONTRIBUTING_en-us.md) before making a pull request.

## License
MIT
