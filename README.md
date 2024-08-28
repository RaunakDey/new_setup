# new_setup
Setting up new MacBook M3


### Few checks to see what it comes with

First check python version. Mine came with 3.9. 
```
which python3
which pip3
python --version
```

Next check which packages come installed.
```
pip list 
```

I preferred python 3.11.9 (and I installed it by simply downliading it) -- brew does not come now a days as env management in MacOS. So after downloading please check.
```
/Library/Frameworks/Python.framework/Versions/3.11/bin/python3 --version
```
You can use symlink to hardcode python or python3 into this new python (yes you can change it later)
```
sudo ln -sf /Library/Frameworks/Python.framework/Versions/3.11/bin/python3 /usr/local/bin/python3
```
I recommend setting up aliases instead. In the ~/.zshrc
 file please set up the alises.
```
alias python="/Library/Frameworks/Python.framework/Versions/3.11/bin/python3"
alias python3="/Library/Frameworks/Python.framework/Versions/3.11/bin/python3"
alias pip="/Library/Frameworks/Python.framework/Versions/3.11/bin/pip3"
alias pip3="/Library/Frameworks/Python.framework/Versions/3.11/bin/pip3"
```
Set it to source (now you will be able to call it from anywhere)
```
source ~/.zshrc
```

(Similarly I could also have used the bash to do this, I am using just the default case)

Now I can keep on using pip (my favourite package manager) to keep on installing stuff to the global environment without any problem.


### Setting up a venv 




### Setting up my GitHub (private ssh keys)



### Setting up my anaconda environment and VSCode
Simply downlaod it. This python will not be the same as the python in the alias which I had set up previously. I can manually choose the interpreter of which python for VSCode, but all the packages needs to be redone for both Jupyter and VSCode.
I suggest set up jupyter outside anaconda as well. (I will rarely use anaconda). Please note that the jupyter from conda or miniconda or anaconda is different from the one installed through pip.


### Setting up environmental PATH variables (global)




