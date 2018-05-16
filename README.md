# Hacks to share

## Workflow for coding in Jupyter lab and publishing to .py files.
Coding in Jupyter lab is great, but its a pain to automate calling notebooks. 
nbconvert can convert .ipynb files to .py files, but any magic lines will cause python.exe to choke.
Using some nifty functions from  [rgerkin](https://github.com/rgerkin), we can have a pretty simple workflow:

    [Edit test.ipynb in Jupyter lab]
    ./pyconvert.sh test.ipynb
    python test.py
