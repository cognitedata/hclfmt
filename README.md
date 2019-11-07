# HclFmt :: Revivified

This project is a fork from the original [fatih/hclfmt](https://github.com/fatih/hclfmt) .  Please see that project for reference.

HclFmt is meant to be a very simple tool for use in text editors to keep your `.hcl` files squared away to the latest of hashicorp's standards.

Notable differences between the original project and this iteration is the sourcing of the `hclparse` and `hclwrite` packages from the [hashicorp/hcl2](https://github.com/hashicorp/hcl2) codebase.  Some recent developments in hcl were not captured in the `hcl/printer` package of [hashicorp/hcl](https://github.com/hashicorp/hcl).

# hclfmt [![Build Status](http://img.shields.io/travis/fatih/hclfmt.svg?style=flat-square)](https://travis-ci.org/fatih/hclfmt)

hclfmt is a command to format and prettify HCL files. It's similar to the
popular `gofmt` command. Hook it with your favourite editor or use it from the
command line.

## Install

If you have Go installed just do:

```bash
go get github.com/fatih/hclfmt
```

## Editor integration

* [vim-hclfmt plugin](https://github.com/fatih/vim-hclfmt)
* [atom-hclfmt](https://atom.io/packages/hclfmt)

## Usage

The usage is similar to `gofmt`. If you pass a file it prints the formatted
output to std output:

```bash
$ hclfmt config.hcl
```

You can pass the `-w` flag to directly overwrite your file:

```bash
$ hclfmt -w config.hcl
```

If no arguments are passed, it excepts the input from standard input.


## License

The BSD 3-Clause License - see
[`LICENSE`](https://github.com/fatih/hclfmt/blob/master/LICENSE) for more
details

