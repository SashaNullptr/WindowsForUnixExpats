# Windows For Unix Expats

![Build Status](https://travis-ci.org/SashaNullptr/WindowsForUnixExpats.svg?branch=master)

## Who Is This Guide For?

Unix developers making the transition into Windows development.

## Things You'll Need

* MkDocs
* Cinder Theme for MkDocs

Assuming you have [Chocolatey](https://chocolatey.org/) installed, the following PowerShell script should install all required pre-requistes.

```shell
choco install -y python3
choco install -y mkdocs
python -m pip install mkdocs-cinder
```
You may also need to add the `C:\Python37\Scripts` folder to the PATH in order for MkDocs to be usable from the command line.

```shell
env:Path = "C:\Python37\Scripts";
```

## Building Docs and Pushing to GitHub

MkDocs supports building docs and updating GitHub pages fairly easily. Simply run `mkdocs gh-deploy -r $REMOTE_BRANCH_NAME -b $LOCAL_BRANCH_NAME`
and documentation will be built and uploaded to the `gh-pages` branch for
this project.
