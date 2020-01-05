# Setup notes for the Shell/Python/Git workshop on January 13, 2020

Please complete the setup tailored to your platform [as described at the bottom of the course web page.](https://carpentries-uconn.github.io/2020-01-13-uconn/)  Here are some notes regarding that process.

The installation notes on the course page *suggest* the use of the [anaconda distribution](https://www.anaconda.com/distribution/), but we **require** use of the Python 3.x version of this distribution for the course.

We will be using [jupyter lab](https://jupyter.org), which provides an integrated environment for code, graphics, and text.  Jupyter lab is installed by default along with the anaconda distribution so you don't need to do anything special to obtain it.  After you complete the steps described in the course web page, you should open a *bash* shell (a terminal under MacOSX or Linux, or the git-bash shell you installed on windows) and type

```
$ jupyter lab
```

If jupyter is properly installed, a window should open on your web browser showing the jupyter interface.
If this *does not work*, drop a line to *Jeremy Teitelbaum at Uconn dot edu* so we're not taken by surprise at the workshop.  

Once you do (or don't) confirm that jupyter opens, close the terminal window where you started it as well as the tab in your browser that it opened.

We intend to use the version of git that is integrated with jupyter but to use it requires a little more configuration.  Open a terminal window (or the git-bash window) and type the following:

```
$ conda install nodejs
```
Answer yes to any prompts.
This installs nodejs, a javascript software package that jupyter uses to control your browser.

Now we will install the jupyterlab-git extension. In a terminal window (the same one you used above is fine),
type:

```
pip install --upgrade jupyterlab-git
jupyter lab build
```

This may take some time as the jupyter program needs to be recompiled with the git library added.
Be patient! 

There is one more step required, but we will do that at the workshop.

### Data Files

The exercises in the course make use of some data files and you should download those so they are available. Put them
on your desktop or somewhere else you can find them easily.

- [data-shell for the shell lesson](https://swcarpentry.github.io/shell-novice/data/data-shell.zip)
- [gapminder data for the python lesson](https://swcarpentry.github.io/python-novice-gapminder/files/python-novice-gapminder-data.zip)
- [full gapminder data](./data/gapminder_data.csv)

### Additional Help

This [pandas cheat sheet](./data/Pandas_Cheat_Sheet.pdf) is useful to have around.

See you soon!





