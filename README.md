# md5check

## Description

Code to check md5 signatures of files on any kind of machine. 

## Prerequisites

 * [md5sum](https://doc.ubuntu-fr.org/md5sum) for linux 
 * [md5](https://md5.soft32.fr/) for mac 

## How to use ? 

```
Usage: bin/md5check [--help] [--input_dir INPUT_DIR] [--extension EXTENSION] [--md5 MD5]

Optional arguments:
    -h      --help
                Print this help and exit.


Required arguments:
    -i      --input_dir
                Directory contains sample directory. 
                Each sample directory must be contain one or plus
                X file-s and the corresponding X.md5. 
                X is define by '--extension' argument.

    -x      --extension
                With '--input_dir' argument.
                Looking only for file with the precised extension.
                [ Default : fastq.gz ]

    -m      --md5
                File with alpha-numerical footprint of each files to
                check. 
```

### Examples 

```
bin/md5check --md5 examples/

bin/md5check --md5 examples/fileMD5.txt 
```

## Bugs

* Submit problems or requests here: https://gitlab.com/md5check/issues

## Authors

Written by Corentin Hochart (corentin.hochart.pro@gmail.com)
