# Deploy locally

This site is a Hugo site which uses the blowfish theme as a git submodule. Make
sure you have a recent version of `hugo` installed.

The themes are installed as sub-modules, so make sure to use the following command:


```
git clone --recurse-submodules --shallow-submodules https://github.com/tpf/tprf-hugo-site
hugo serve
```
