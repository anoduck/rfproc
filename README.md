<h1 align="center">Welcome to rfproc 👋</h1>
<p>
  <img alt="Version" src="https://img.shields.io/badge/version-0.0.8-blue.svg?cacheSeconds=2592000" />
  <a href="#" target="_blank">
    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg" />
  </a>
</p>

> A bash script to batch process data files from rtl_433.

## Install

To install simply copy `rfproc` to somewhere in your path. Currently, `~/.local/bin` seems to be a popular choice, but if you have `~/bin` in your path, it works all the same.

You do need to have bash, awk, [fd](https://github.com/sharkdp/fd), and rtl_433 installed.

```sh
cp rfproc ~/.local/bin
```

## Usage

```sh
rfproc --help
Program : rfproc  by 11767-anoduck@users.noreply.gitgud.io
Version : v0.0.8 (2024-04-17 02:17)
Purpose : A script to aid processing of rtl_433 generated files
Usage   : rfproc [-h] [-q] [-v] [-f] [-l <log_dir>] [-t <tmp_dir>] [-i <input>] [-i <script>] <action>
Flags, options and parameters:
    -h|--help        : [flag] show usage [default: off]
    -q|--quiet       : [flag] no output [default: off]
    -v|--verbose     : [flag] also show debug messages [default: off]
    -f|--force       : [flag] do not ask for confirmation (always yes) [default: off]
    -l|--log_dir <?> : [option] folder for log files   [default: /home/***REMOVED***/log/rfproc]
    -t|--tmp_dir <?> : [option] folder for temp files  [default: /tmp/rfproc]
    -i|--input <?>   : [option] input folder for processing  [default: /home/***REMOVED***/Sandbox/ISM-Research/test-bin]
    -i|--script <?>  : [option] name of shell script to write demod commands to  [default: rfproc.sh]
    <action>         : [choice] action to perform  [options: proc,decode,convert,clean,check,env,update]

### TIPS & EXAMPLES
* use rfproc proc to ...
  rfproc proc
* use rfproc clean to ...
  rfproc clean
* use rfproc clean to ...
  rfproc clean
* use rfproc clean to ...
  rfproc clean
* use rfproc check to check if this script is ready to execute and what values the options/flags are
  rfproc check
* use rfproc env to generate an example .env file
  rfproc env > .env
* use rfproc update to update to the latest version
  rfproc update
* >>> bash script created with pforret/bashew
* >>> for bash development, also check out pforret/setver and pforret/progressbar
```

## Author

👤 **Anoduck**

* Website: http://anoduck.github.io
* Github: [@anoduck](https://github.com/anoduck)

## Show your support

Give a ⭐️ if this project helped you!

***
_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_
