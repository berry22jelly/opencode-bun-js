# Make sure bun is installed

Install Bun if you haven’t already:
```sh
curl -fsSL https://bun.sh/install | bash
```
Or follow instructions at [https://bun.sh/docs/installation](https://bun.sh/docs/installation).

# Clone opencode

Clone the opencode repository:
```sh
git clone https://github.com/anomalyco/opencode
cd opencode
```

# Add build files

## Edit `package.json`

Add the following scripts to `opencode/packages/opencode/package.json` (make sure to edit this package.json, not the root one):

```json
"scripts": {
    "build:js": "bun run script/build-js.ts",
    "start:js": "bun run dist/js/src/index.js",
    // ...any other scripts
}
```
Add or merge with existing `"scripts"` as needed.

## Add `build-js.ts`

Copy `build-js.ts`(in this repo) to `opencode/packages/opencode/script/build-js.ts`.  

# Build & Run

To build the JS bundle:
```sh
cd opencode/packages/opencode
bun run build:js
```

To start your application:
```sh
bun run start:js help
```
