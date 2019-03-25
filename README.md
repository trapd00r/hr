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

    -c,    --char       Character to use
    -s,    --size       Number of columns
    -pre,  --pre        Pad the left side with whitespace n
    -post, --post       Pad the right side with whitespace n
    -fg,   --fg         Foreground color to use, int 0-255
    -bg,   --bg         Background color to use, int 0-255
    -b,    --bold       Use bold
    -i,    --italic     Use italics
    -u,    --underline  Use underline
    -r,    --reverse    Use reverse video

    -h,    --help       Display this help and exit
    -m,    --man        Display the manual and exit
    -v,    --version    Display version info and exit

# EXAMPLES

    # display a yellow underlined bar using the default '=' character
    hr -fg 220 --underline
![example01.png](/extra/example01.png)



    # display a red solid bar padded by 10 columns from right and left
    hr -fg 160 -c ▀ --pre 10 --post 10
![example02.png](/extra/example02.png)

    # display a solid grey, thick bar using ascii character _ and the bold,
    # underline and reverse video attributes

    hr -fg 240 -c_ -bur
![example03.png](/extra/example03.png)

    # display a bar made of dots, with 5 column spacing one each size
    # and 20 columns wide.

    hr -fg 197 -c· -pre 5 -post 5 -size 20
![example04.png](/extra/example04.png)

    # use all options at once, because why not?
    hr -c ! -fg 52 -bg 196 -biur -s 70 -pre 5 -post 5
![example05.png](/extra/example05.png)

    # use several characters to form a bar using arithmetics
    hr -c "  japh  " -fg 1 -bg 0 -b -s $(($COLUMNS / 8))
![example06.png](/extra/example06.png)

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
