## action
- (single)
  - store (DEFAULT)
  - store_const/true/false (flag)
- (multiple)
  - append/_const
    - (append_const + dest)
  - count (verbose-level)
  - extend (3.8+)
- (misc)
  - help, version
## parser.add_argument()
- (basic)
  - name/flags/alias (pos, -short, --long)
  - nargs (N, ?, *, +)
  - default (fallback)
  - type (auto-convert-callback)
- (advanced)
  - action
    - const (default-for-action)
  - dest (var-name)
- (misc)
  - required
  - choices
  - help
    - metavar (placeholder-in-help)
## (metaphor)
- args: positional, keyword(option), default
- argparse (arg-parse)
  - ArgumentParser (argument-parser)
    - add_argument (argument)
    - parse_args (args-parse)
  + ArgumentParser => argparse
  + argument(parameter): \
      ArgumentParser, add_argument
  + arg(argument): \
      argparse, parse_args


# argparse
## ArgumentParser
### (normal-usage)
- add_argument()
- parse_args() \
    parse_known_args() \
    parse_intermixed_args() \
    parse_known_intermixed_args()
- set_defaults() \
    get_default() 
### (advanced)
- add_subparsers()
- add_argument_group() \
    add_mutually_exclusive_group()
### (override)
- convert_arg_line_to_args()
## Action


----
----
----
### todo
- arguments-style
  - abbrev
    - --long=val
    - -abcdefg
    - /dos-style
    - -- -escape-normal-val
    - -prefixmatch
  - file-support
    - @argfile_prefix
    - `-` stdin/stdout 
- subparser (cmd)
- argument_group
  - help, exclusive
