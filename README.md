# pebble-platform-sdk
Tool to compile and package pebble packages/apps/watchfaces compiling with different sdk version per platform

## Installation
```shell
npm install pebble-platform-sdk --save-dev
```

This will also add the following line to your package.json in scripts:

```javascript
"build": "pebble-platform-sdk aplite=3.13.1 basalt=3.13.1 chalk=3.13.1 diorite=4.0 emery=4.2"
```

Edit package.json, and replace the versions in the above line to the desired sdk versions for each platform

## Usage
```shell
npm run build
```

The output will be `${package.name}-${package.version}.pbw` in the project directory
