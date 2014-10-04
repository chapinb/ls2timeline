ls2timeline
===========

Create a timeline from ls output

# About

This tool will read input from a text file containing information from the ls command. This input should be generated by running `ls -laR`. 

In example, you could run `ls -laR / > ls-output.txt` then convert it using `python ls2timeline.py ls-output.txt ls-output.csv`.

The tool will only list non-directory and non-linked files for stability purposes at this time.

# Dependencies

Requires Python 2.7

# Usage

    usage: ls2timeline.py [-h] [-v] source target
    
    Convert file listing output into CSV timeline. 
    
    **Ensure input file was generated by running `ls -laR` against the desired partition**
    
    positional arguments:
      source         text file to process
      target         output csv file
    
    optional arguments:
      -h, --help     show this help message and exit
      -v, --version  show program's version number and exit
  
# Future
* Add mactime output support
* Add support for linked files
* Add support for directory entries
