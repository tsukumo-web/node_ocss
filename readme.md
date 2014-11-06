# ocss


## About

Optimization and clean up tool for CSS


## Why

### Optimize
CSS rules may be written in many forms and in many places causing
overlap and unexpected results.

### Clean up
CSS files can become unruly after many iterations of trial and error.

### Validation
Verify that css files are properly formatted and detect issues - most
browsers will ‘swallow’ issues in css rendering it a difficult language
to debug.


## How to

```sh
$ [sudo] npm i -g ocss
```

```sh
Usage:
    ocss [ [-h] | [-v] | [-i [-o]] | [-o] | [-w [-s]] | [INPUT] [OUTPUT] ]
    [-n] [-a | -g | -c]

Options:
    -h, --help      : Help
    -v, --version   : Version
    # Files
    -i, --input     : Input file        [FILE]      Default: STDIN
    -o, --output    : Output file       [FILE]      Default: INPUT (STDIN > STDOUT)
*   -w, --watch     : Watch folder      [DIR:DIR]   Default: .:css
*   -s, --suffix    : Suffix for output [STR]       Default: .css
    # Style
*   -n, --newline   : Bracket on newline
*   -a, --alpha     : Order tags by alphabet        Default
*   -g, --group     : Order tags by type
*   -c, --custom    : Specify a custom ordering
    # Branding
    -b, --banner    : Specify banner                Default: Generated with OCSS: TIMESTAMP

Args:
    INPUT:  alias to input
    OUTPUT: alias to output

* Not yet implemented
```

Files
```sh
$ ocss a.css

    --or--

$ ocss a.css b.css
```

stdin / stdout
```sh
$ “.a{margin:10px}” | ocss
>
> .a {
>   margin: 10px;
> }
>
```


## License

The MIT License
(See license)


## Authors
Chris Kelley (Tsukumo) <tsukumo.code+web(at)gmail.com>

