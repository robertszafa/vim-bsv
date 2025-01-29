# Vim plugin for Bluespec SystemVerilog (BSV)

## Installation using Lazy in neovim
```lua
{
  "robertszafa/vim-bsv",
  ft = { "bsv", "bc" },
},
```

## Snippet support with blink.cmp

Add `snippets/bsv.json` to the `~/.config/snippets/` directory, or wherever your neovim config lives.
If you do not have this file already, also add `package.json` to the `~/.config/snippets/` directory and paste the following in:
```json
{
  "name": "personal-snippets",
  "contributes": {
    "snippets": [
      { "language": "bsv", "path": "./bsv.json" }
    ]
  }
}
```
If you do already have this file with other vs-code snippets, then you just need to add the following field to the `snippets` array:
```json
      { "language": "bsv", "path": "./bsv.json" }
```

