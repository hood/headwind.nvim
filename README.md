# headwind.nvim

Port of the [VSCode headwind plugin](https://marketplace.visualstudio.com/items?itemName=heybourn.headwind)

This is still alpha level software... use with caution.

## Install

```lua
-- Packer
use "steelsojka/headwind.nvim"
```

## Setup

```lua
require "headwind".setup {
  -- options here
}
```

### Options

#### sort_tailwind_class

A list that determines Headwind's defauls sort order

#### remove_duplicates

Headwind will remove duplicate class names by default. This can be toggled on or off. This defaults to `false`.

#### prepend_custom_classes

Headwind will append custom class names by default. They can be prepended instead. Defaults to `true`.

## Usage

Headwind doesn't do anything... you must call the API methods. This allows users to control when they want things to happen.

### Api

#### buf_sort_tailwind_classes([bufnr], [opts])

Sorts all tailwind class matchers in the buffer and edits them in place.

- `bufnr`: The buffer to use. Will use active buffer if not provided.
- `opts`: Options that will override the global and user defined options.
