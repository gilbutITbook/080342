If you run this command from the book in the Mac Terminal:

  $ echo 2021-{01..12}-01 | xargs -n1 date +%B -d

it may fail with this result:

  date: illegal time format

That's because the Mac's "date" command is different from the Linux
command. Specifically, the option -d has a different meaning on the
Mac. A working command on the Mac is:

  $ echo 2021-{01..12}-01 | xargs -n1 -I@ date -j -f %Y-%m-%d @ +%B

If interested, you can install the Linux version of the "date" command
using Homebrew, by installing the package "coreutils". The command is
named "gdate".
