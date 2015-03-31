# NAME

Code::TidyAll::Plugin::PgFormatter - Code::TidyAll plugin for pg\_format

# SYNOPSIS

    In your tidyall config:

    [PgFormatter]
    select = **/*sql
    ; affects formatted output, defaults for pg_format shown
    argv = --function-case 0 --keyword-case 2 --spaces 4

# DESCRIPTION

Code::TidyAll::Plugin::PgFormatter is a plugin for Code::TidyAll that will call
pg\_format from the [https://sourceforge.net/p/pgformatter/](https://sourceforge.net/p/pgformatter/) project, and
nicely-format your SQL files.

# INSTALLATION

Following the installation instructions in the github project page:
<https://github.com/darold/pgFormatter>

Note that CGI is required by pg\_format, you may need to install it in
more-recent versions of perl.

    cpanm CGI

# CONFIGURATION

- argv

    Arguments to pass to pg\_format.  See the pgFormatter documentation for
    command-line options.

# AUTHOR

Andy Jack <andyjack@cpan.org>

# COPYRIGHT

Copyright 2015- Andy Jack

# LICENSE

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.

# SEE ALSO

[Code::TidyAll](https://metacpan.org/pod/Code::TidyAll)
