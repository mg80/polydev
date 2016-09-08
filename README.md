# polydev

polydev is the Polymer DevTools Extension - a tool to help develop Polymer and
custom elements.

## Release Installation

The release version of polydev is available on the Chrome Web Store:

https://chrome.google.com/webstore/detail/polymer-devtools-extensio/mmpfaamodhhlbadloaibpocmcomledcg

## Development

### Building

polydev must be built before running. The build step externalizes inline scripts
for CSP compliance, and copies some dependencies into convenient locations.

To build, run `npm run build`:

    > npm run build

The built project is available at `build/polydev`.

### Installation

 1. Create a new Chrome profile
 2. Navigate to chrome://extensions
 3. Check the "Developer mode" checkbox
 4. Click "Load unpacked extension..."
 5. Choose `/polydev/build/polydev`

### Dev flow

When changing files in src/ the dev workflow should work cover most use cases.

    > npm run dev

Depending on the change you can either then close and reopen the devtools, or if
you've made a change to the content-script or to element-zones, you must reload
both the extension and any page you're testing it on.
