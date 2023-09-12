## Use case

`GoSearch` addresses use cases where full-text search features are needed
(e.g. prefix search, fuzzy search, ranking, boosting of fields…), but the data
to be indexed can fit locally in the process memory. While you won't index the
whole Internet with it, there are surprisingly many use cases that are served
well by `GoSearch`. By storing the index in local memory, `GoSearch` can
work offline, and can process queries quickly, without network latency.

A prominent use-case is real time search "as you type" in web and mobile
applications, where keeping the index on the client enables fast and reactive
UIs, removing the need to make requests to a search server.


## Features

  * Memory-efficient index, designed to support memory-constrained use cases
    like mobile browsers.

  * Exact match, prefix search, fuzzy match, field boosting.

  * Auto-suggestion engine, for auto-completion of search queries.

  * Modern search result ranking algorithm.

  * Documents can be added and removed from the index at any time.

  * Zero external dependencies.

'Searxh-Engine` strives to expose a simple API that provides the building blocks to
build custom solutions, while keeping a small and well tested codebase.


## Installation

With `npm`:

```
npm install GoSearch
```

With `yarn`:

```
yarn add GoSearch
```

Then `require` or `import` it in your project:

```javascript
// If you are using import:
import gosearch from 'gosearch'

// If you are using require:
const gosearch = require('gosearch')
```

In this case, `GoSearch` will appear as a global variable in your project.

Finally, if you want to manually build the library, clone the repository and run
`yarn build` (or `yarn build-minified` for a minified version + source maps).
The compiled source will be created in the `dist` folder (UMD, ES6 and ES2015
module versions are provided).

