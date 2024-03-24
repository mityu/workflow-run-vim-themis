# gha-workflow-run-vim-themis

This is a GitHub Actions workflow to run Vim/Neovim plugin tests powered by themis.vim.

This action does:
1. Checkout the plugin repository using [actions/checkout](https://github.com/actions/checkout).
2. Setup Vim/Neovim using [thinca/action-setup-vim](https://github.com/thinca/action-setup-vim).
3. Show Vim/Neovim version.
4. Setup themis.vim using [actions/checkout](https://github.com/actions/checkout).
5. Run unit tests by `themis --reporter tap`.

## Usage

## Workflow inputs

**`os`** (Required)

The operating system to run tests on.

**`vim_type`** (Required)

Specify the type of Vim.  This parameter is passed to `vim_type` input of `thinca/action-setup-vim` directly.

**`vim_version`** (Required)

Specify the Vim version.  This parameter is passed to `vim_version` input of `thinca/action-setup-vim` directly.

**`download`** (Optional)

Specify how to prepare Vim binary.  This parameter is passed to `download` input of `thinca/action-setup-vim` directly.

For the details of inputs related to thinca/action-setup-vim, refer to [the README of thinca/action-setup-vim](https://github.com/thinca/action-setup-vim/blob/master/README.md).
