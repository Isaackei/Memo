Set up Virtual environment for Mac OS

Two add-on are require:

1. Virtualenv

   `pip3 install virtualenv`

2. Virtualenvwrapper 

   `pip3 install virtualenvwrapper`



Next, prepare a file with any name you like, mine is `.virtualenvs`.

And, prepare another document if it is not exist, named: `.bash_profile`. (Technically, those name can be personal preference)

Both new create or exist files should be better located after ~ path (default path)



Edit `.bash_profile` and write in three lines of code. **Important: make sure those three lines follow the order**

1. `export WORKON_HOME=~/.virtualenvs`[^1]

2. `export VIRTUALENVWRAPPER_PYTHON=/Library/Frameworks/Python.framework/Versions/3.6/bin/python3`[^2]

3. `source /Library/Frameworks/Python.framework/Versions/3.6/bin/virtualenvwrapper.sh`

   [^1]: Set diretory for virtual environment while create, also reference for  `workon` command to show all virtual environment.
   [^2]: Set default python3 environment.
   [^3]: Import and update virtualenvwrapper



Source this .bash_profile should work perfectly fine.

Now, you can

> workon
>
> mkvirtualenv
>
> rmvirtualenv
>
> deactivate  

if you have probelm with oh-my-zsh, while virtualenv is not showing at the left of your terminals. 
cd

find 

defined POWERLEVEL9K_LEFT_PROMPT_ELEMENTS || POWERLEVEL9K_LEFT_PROMPT_ELEMENTS=(virtualenv context dir vcs)
  defined POWERLEVEL9K_RIGHT_PROMPT_ELEMENTS || POWERLEVEL9K_RIGHT_PROMPT_

add "virtualenv" inside (context dir vcs) 



