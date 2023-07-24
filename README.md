# Fivemanage API SDK for FiveM

This is the official Fivemanage API SDK for FiveM. It is written in Javascript and Lua.

## Installation
Download the latest release from the [releases](https://github.com/fivemanage/sdk/releases). Make sure it is the `fivemanage_lib.zip
` file.

## Usage
Add the following to your `server.cfg`:
```
set FIVEMANAGE_IMAGE_TOKEN your_token
```
This is the token for image uploading

You can now call events or exports.

### Client Exports
```lua
exports.fivemanage_lib:takeImage()

-- With metadata

exports.fivemanage_lib:takeImage({
    name = "My image",
    description = "This is my image",
    -- or any other field you want
})
```

### Server Exports
```lua
exports.fivemanage_lib:takeServerImage(src)

-- With metadata

exports.fivemanage_lib:takeServerImage(src, {
    name = "My image",
    description = "This is my image",
    -- or any other field you want
})
```

