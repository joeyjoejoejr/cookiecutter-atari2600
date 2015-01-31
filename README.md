cookiecutter-atari2600
===========

This is a template that creates a project set up with a basic kernal, playfield
graphic, and make commands to to do basic tasks.

```bash
make       # build the project into a binary in the dist directory

make run   # build the project and run it in stella (set variable)

make clear # clean up files
```

This also has a bitmap to data-table converter in the bin directory, you must
have dasm on your path.


Usage
-----

You will need to install DASM (Build from source for nix systems):
[dasm source](http://sourceforge.net/p/dasm-dillon/code/HEAD/tree/)

You will need to install Stella: http://stella.sourceforge.net/

You need [cookiecutter](https://github.com/audreyr/cookiecutter), a tool to create projects from project
templates. Once installed (in a virtualenv or just with `pip install
cookiecutter`), you can use the following command:

    cookiecutter https://github.com/joeyjoejoejr/cookiecutter-atari2600.git
    cd your-project
    # edit your makefile to include the path to stella
    make run
