[![LICENSE](https://img.shields.io/badge/license-MIT-orange.svg)](LICENSE)
[![Go Report Card](https://goreportcard.com/badge/github.com/arxdsilva/XML-Comp)](https://goreportcard.com/report/github.com/arxdsilva/XML-Comp)
[![codebeat badge](https://codebeat.co/badges/1600adbb-27a3-4c3b-803e-818e1834b51a)](https://codebeat.co/projects/github-com-arxdsilva-xml-comp)
[![GoDoc](https://godoc.org/github.com/arxdsilva/xml-comp?status.png)](https://godoc.org/github.com/arxdsilva/xml-comp)
[![Top Level Coverage](https://coveralls.io/repos/github/ArxdSilva/XML-Comp/badge.svg?branch=master)](https://coveralls.io/github/ArxdSilva/XML-Comp?branch=master) / [![comparer coverage](https://gocover.io/_badge/github.com/ArxdSilva/xml-comp/comparer?0 "comparer coverage")](http://gocover.io/github.com/ArxdSilva/XML-Comp/comparer)
[![Travis Build Status](https://api.travis-ci.org/ArxdSilva/XML-Comp.svg?branch=master)](https://travis-ci.com/arxdsilva/xml-comp)

## XML-Comparer
This package is a command line tool that provides the capability of comparing two directories and outputs files with differences between them, including: missing Files, missing Folders and missing Tags of .xml files. It was made to help [RimWorld](http://rimworldgame.com/)'s [community translators](https://github.com/ludeon)(1) to know what was modified on the last XML updates and to let them keep in track of what they need to add/remove from what has been done.

(1) and maybe other indie games that uses XML

### Installing
```
$ go get github.com/ArxdSilva/XML-Comp
```

### Running
```shell
$ XML-Comp -comp -original /path/to/language/english -translation /path/to/language/translation
```

### How this works? - RimWorld translator
You need two paths that we call "original" & "translation", which are described bellow:
- "original": Full path directory of your RimWorld English folder

My path - as an example: "original" = **/Users/arthur/Library/Application Support/Steam/steamapps/common/RimWorld/RimWorldMac.app/Mods/Core/Languages/English**
- "translation": Full path directory of your RimWorld ~Language~ folder cloned from [GitHub](https://github.com/ludeon)

Me again: "translation" = **/Users/arthur/Github/RimWorld-PortugueseBrazilian**

With these paths in hand you run our program and It will let you know in a `missingSomethieng.txt` file what is missing and where in your translation! That simple!

#### XML-Comp CLI Usage (needed Go 1.7+)
```shell
$ git clone github.com/arxdsilva/xml-comp
$ cd xml-comp
$ go install
$ xml-comp help
```

#### To Do - Check our [Issues](https://github.com/ArxdSilva/XML-Comp/issues) & [Milestones]()
- [GUI](https://github.com/ArxdSilva/XML-Comp/issues/10)
- [Installer](https://github.com/ArxdSilva/XML-Comp/issues/12)
