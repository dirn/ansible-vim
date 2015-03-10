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

To install gVim (MacVim on OSX):

    vim_install_gvim: true

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: dirn.vim

License
-------

MIT

Author Information
------------------

This role was created by [Andy Dirnberger](https://github.com/dirn).
