YouCompleteMe: a code-completion engine for Vim
===============================================

## Disclaimer
Go to original repo [here](https://github.com/Valloric/YouCompleteMe)

## what new in this repo ?
This repo works for pyenv version of python, which works on my mac


```
echo $PATH
/Users/ldong/.rvm/gems/ruby-2.1.2/bin:/Users/ldong/.rvm/gems/ruby-2.1.2@global/bin:/Users/ldong/.rvm/rubies/ruby-2.1.2/bin:/Users/ldong/.pyenv/shims:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin:/opt/X11/bin:/usr/texbin:/usr/bin:/bin:/usr/sbin:/sbin:/usr/local/bin:/opt/X11/bin:/Users/ldong/.rvm/bin


echo $PYTHONPATH
:/Users/ldong/.pyenv/shims/python

```

You also have to add this to `.vimrc`

`let g:ycm_path_to_python_interpreter = '/Users/ldong/.pyenv/shims/python'`

Read More [here](https://gist.github.com/ldong/9a22fe008e896d574ade)
