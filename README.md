# To reproduce the bug
`npm run dev` then navigate to localhost:3000

## Solution

* add `  serverDependenciesToBundle: ["react-charts", "d3-time-format"],` to remix.coonfig.js

This is a ESM module issue, see docs for details:

https://remix.run/docs/en/v1/pages/gotchas#importing-esm-packages
