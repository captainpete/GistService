GistService
===========

A simple OS X service for easily posting text or files to Gist on Github.

Installation
------------

Just copy GistService.service to ~/Library/Services, or /Library/Services if you want it for all users.

From source:

    rake install      # Install for this user
    rake install_all  # Install for all users


Authentication
--------------

By default, GistService will post your Gists anonymously, but if you'd like, you can set it up to paste as yourself; just run:

    git config --global github.user "your github username"
    git config --global github.token "your github token"

You can obtain these values on [your Github Settings page, under 'Personal Access Tokens'](https://github.com/settings/applications#personal-access-tokens).

Acknowledgements
----------------

GistService was written by Andy Matuschak <andy@andymatuschak.org>

But it's just a wrapper around gistpaste, a script by David Blevins <dblevins@visi.com>. Thanks, David!