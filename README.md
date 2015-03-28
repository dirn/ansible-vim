Vim
===

[![Build Status](https://travis-ci.org/dirn/ansible-vim.svg?branch=master)](https://travis-ci.org/dirn/ansible-vim)

An Ansible role to install [Vim](http://www.vim.org/).

Requirements
------------

This role works on OS X and Debian-based OSes. If using OS X, make sure you have
[Homebrew](http://brew.sh/) installed before running the role. If you're looking
for a role to handle it for you, check out
[dirn.homebrew](https://github.com/dirn/ansible-homebrew).

Role Variables
--------------

Several variables are available to configure the role.

To control if gVim (MacVim on OSX) is installed:

    vim_install_gvim: true

To control if [Neovim](http://neovim.org/) is installed:

    vim_install_nvim: false

To control if [NeoBundle](https://github.com/Shougo/neobundle.vim) is installed:

    vim_install_neobundle: false

To control if [Pathogen](https://github.com/tpope/vim-pathogen) is installed:

    vim_install_pathogen: false

To control if [Plug](https://github.com/junegunn/vim-plug) is installed:

    vim_install_plug: false

To control if [Vundle](https://github.com/gmarik/Vundle.vim) is installed:

    vim_install_vundle: false

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
        - role: dirn.vim
          vim_install_gvim: true
          vim_install_nvim: true
          vim_install_neobundle: true

License
-------

MIT

Author Information
------------------

This role was created by [Andy Dirnberger](https://github.com/dirn).
