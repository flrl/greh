# greh - global regular expression highlighter

Print lines from input files, highlighting the ones that match patterns.

Example:

    make 2>&1 | greh -i --red error: --yellow warning:

> Which pattern syntax is used?

Perl's one. See `perldoc perlre` for details.

> How is this different from `hgrep` or `grep --color`?

* `grep --color` prints lines that match, and highlights the matching
  substrings within those lines.
* ... as does `hgrep`.
* `greh` prints all lines, and highlights the ones that match.
