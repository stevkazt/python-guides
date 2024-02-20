# Pyenv

Pyenv, standing for "Python Version Management," is a lightweight and user-friendly tool that lets you seamlessly switch between multiple Python versions on your system, like a toolbox for different Python flavors. Whether you need the latest features of Python 3.11 or prefer the stability of 2.7, pyenv helps you manage them all independently. No messy system-wide installations or conflicts!

 It operates silently in the background, setting up individual environments for each version and keeping them separate. This empowers you to work on different projects requiring specific Python versions without any hassle. Need to test code against an older version? Just switch with a simple command! Pyenv also integrates with virtual environments, further enhancing your project isolation and development flexibility. So, if you juggle various Python projects or want to explore different versions, pyenv is your key to effortless Python version management.

 ## Setting it up!

1. Install pyenv:
   
    `brew install pyenv`

2. Install pyenv-virtualenv:
   
    `brew install pyenv-virtualenv`

3. Add pyenv shims and activate pyenv, add the next lines to `~/.zshrc`:

    `export PATH=/opt/homebrew/bin:$PATH`

    `eval "$(pyenv init --path)"`

    `eval "$(pyenv init -)"`

    `eval "$(pyenv virtualenv-init -)"`

    `export PYENV_ROOT="$HOME/.pyenv" [[ -d $PYENV_ROOT/bin ]] \&\& export PATH="$PYENV_ROOT/bin:$PATH"`
    
4. Install a Python version:

    `pyenv install 3.9.6` #Pick the one most suits you
    
5. Create a virtual environment:

    `pyenv virtualenv 3.9.6 my-venv`  # Replace "3.9.6" with your desired Python version

5. Activate the virtual environment:

    `pyenv activate my-venv`

6. Install packages in the virtual environment:

    `pip install <package_name>`

7.  Deactivate the virtual environment:
   
    `deactivate`