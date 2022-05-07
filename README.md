# tig.nvim

[tig](https://github.com/jonas/tig) in your Neovim

## Prerequisites

- Neovim >= 0.5.0
- [tig](https://github.com/jonas/tig)

## Installation

[packer.nvim](https://github.com/wbthomason/packer.nvim)

```lua
use 'ttbug/tig.nvim'
```

## Setup

```lua
require("tig").setup()
```

## Configuration (optional)

Following are the default config for the `setup()`. If you want to override, just modify the option that you want then it will be merged with the default config.

```lua
{
  -- Command Options
  command = {
    -- Enable :Tigui command
    -- @type: bool
    enable = true,
  },
  -- Path to binary
  -- @type: string
  binary = "gitui",
  -- Argumens to tig
  -- @type: table of string
  args = {},
  -- WIndow Options
  window = {
    options = {
      -- Width window in %
      -- @type: number
      width = 90,
      -- Height window in %
      -- @type: number
      height = 80,
      -- Border Style
      -- Enum: "none", "single", "rounded", "solid" or "shadow"
      -- @type: string
      border = "rounded",
    },
  },
}
```

## Lua API

```lua
require("tig").open()
```

## TODO

- Add documentation
