## ansible-osx

Development environment provisioning Mac OS X using [battleschool](https://github.com/spencergibb/battleschool).

### Install

    #if needed
    sudo easy_install pip

    sudo pip install battleschool

### Running battleschool for the first time

    battle --config-file http://somesite/path/to/your/config.yml

As long as your `config.yml` doesn't have a `source.local` section, you don't need to download or create a configuration for the first time.

### Running battleschool

`battle -K`

### Configuration

`mkdir ~/.battleschool`

Put the following in `~/.battleschool/config.yml` and uncomment the items you want intstalled (remove the #)

    ---
    sources:
      git:
        - name: 'osx'
          repo: 'https://github.com/kforsthoevel/ansible-osx'
          playbooks:
            # - zsh.yml
            # - homebrew.yml
            # - cask.yml
            # - dotfiles.yml
            # - oh-my-zsh.yml
            # - chrome-stable.yml
            # - dropbox.yml
            # - handbrake.yml
            # - iterm2.yml
            # - osxfuse.yml
            # - skype.yml
            # - vagrant.yml
            # - virtualbox.yml
            # - vlc.yml

