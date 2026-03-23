# Make sure bun is installed

(placehold)

# Clone opencode

(placehold)

# Add build files

## Edit `package.json`

Add script items into `opencode\packages\opencode\package.json` 

**NOT `package.json` in ROOT directory.**

```
    "build:js": "bun run script/build-js.ts",
    "start:js": "bun run dist/js/src/index.js",
```

## Add `build-js.ts`

Copy `build-js.ts` to `opencode\packages\opencode\script\build-js.ts`

# Build & Run

(placehold)
