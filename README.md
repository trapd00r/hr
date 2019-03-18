# NAME

hr - define a thematic change in the content of a terminal session


# SYNOPSIS

    hr [OPTIONS]

# DESCRIPTION

hr prints a horisontal bar in your terminal. Useful when you run a
chain of commands that might produce a lot of output and you need to
differentiate where a given output is coming from.

![img](/extra/hr.png)


# OPTIONS

    -c,  --char       Character to use
    -s,  --size       Number of columns
    -fg, --fg         Foreground color to use. See Term::ExtendedColor
    -bg, --bg         Background color to use. See Term::ExtendedColor
    -b,  --bold       Use bold
    -i,  --italic     Use italics
    -u,  --underline  Use underline
    -r,  --reverse    Use reverse video

    -h,  --help     display this help and exit
    -v,  --version  display version info and exit

# AUTHOR

    Magnus Woldrich
    CPAN ID: WOLDRICH
    m@japh.se
    http://japh.se
    http://github.com/trapd00r

# COPYRIGHT

Copyright 2019 **THIS APPLICATION**s ["AUTHOR"](#author) and ["CONTRIBUTORS"](#contributors) as listed
above.

# LICENSE

This program is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.
