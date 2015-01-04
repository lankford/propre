[![Gem Version](https://badge.fury.io/rb/propre.svg)](http://badge.fury.io/rb/propre)

Propre
======

![Propre](http://cl.ly/image/3b3M2Q2s2r2r/Image%202014-12-31%20at%204.10.46%20PM.png)

##Introduction

**Propre** is a handy tool written in Ruby to bulk rename your movies using [TheMovieDB](https://www.themoviedb.org/) API.

Propre will extract the title of a movie from it's filename and then rename it based on search result from TMDB.

##Installation

    gem install propre

To use Propre, you need an API Key from TheMovieDB. Get your API key [here](https://www.themoviedb.org/account).

##Usage

    Usage: propre [OPTION]... SOURCE...
        -i, --interactive                Run interactively
        -R, --recursive                  Run recursively
        -V, --video-only                 Search for video files only
        -s, --sanitize                   Sanitize filename before search
        -d, --dotfile                    Don't ignore .dotfile
        -v, --version                    Show version information about this program and quit.
        -h, --help, --usage              Show this help message and quit.

##Changelog

### 0.1.1

  - Fix bug when no movie was found
  - Fix wording

### 0.1.0

  - The first result is now the best match in the list (using similar_text)
  - Results are now ordered by release date
  - Extensions are now in lowercase when renaming (.AVI,.Avi -> .avi)

Disclaimer
----------

This tool was made on my spare time, i'm not responsable of any damages caused to your files
