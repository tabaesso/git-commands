# PATTERNS

\# - The hash marks a comment in our archive
* - Ignores parts of a pattern's name, acting like a wildcard
! - Allows a specific pattern to be excluded. Usually comes with a more general rule
/ - It has different functions depending on your location. At the beginning of the line, ignore a pattern in that directory only, but not in its subdirectories. In the end, it ignores the entire directory tree
\ - Escape character
** - Two asterisks are then used to ignore a specific pattern within a directory tree

Examples:
>Ignore all html files in the repository
*.html

>Except the index.html file
!index.html

>Ignore README in the current directory, but allow subdir/README
/README

>Ignore all files in the build/ directory
build/

>Ignore .txt files in the doc/ directory, but allows subdirectories (doc/server/arch.txt)
doc/*.txt

>Ignore all .pdf files in the doc/ tree
doc/**/*.pdf