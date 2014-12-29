# YouCompleteMe

## Disclaimer

Go to original & latest repo [here](https://github.com/Valloric/YouCompleteMe)

## what new in this repo ?
This repo works for pyenv version of python, which works on my mac


```
which vim
/usr/local/bin/vim

which python
/Users/ldong/.pyenv/shims/python

echo $PATH
/Users/ldong/.rvm/gems/ruby-2.1.2/bin:/Users/ldong/.rvm/gems/ruby-2.1.2@global/bin:/Users/ldong/.rvm/rubies/ruby-2.1.2/bin:/Users/ldong/.pyenv/shims:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin:/opt/X11/bin:/usr/texbin:/usr/bin:/bin:/usr/sbin:/sbin:/usr/local/bin:/opt/X11/bin:/Users/ldong/.rvm/bin

echo $PYTHONPATH
:/Users/ldong/.pyenv/shims/python
```

You also have to add this to `.vimrc`

`let g:ycm_path_to_python_interpreter = '/Users/ldong/.pyenv/shims/python'`

<!-- Read more [here](https://gist.github.com/ldong/9a22fe008e896d574ade) -->


## Update
Sun Dec 28 22:04:04 EST 2014

```
brew install python
brew unlink python && brew link python
brew rm --force macvim
brew install macvim --override-system-vim
```
add this to **.vimrc**

`let g:ycm_path_to_python_interpreter = '/usr/local/bin/python'`

After figure out your brewed python version, go to install.sh, edit

```
"-DPYTHON_EXECUTABLE=/usr/local/Cellar/python/2.7.9/bin/python2.7"
```

to `pyexe`

then run `./install.sh --clang-completer`
