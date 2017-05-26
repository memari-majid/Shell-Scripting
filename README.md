# Shell-Scripting
Logic:
1. Do a basic error check that the program was called with a legal number of arguments,
and if not, print out a “usage” message giving the legal syntax, and exit with failure
status.
2. Make certain the specified ROOT_DIRECTORY is a valid directory, and if not, print an
informative error message and exit with failure status.
3. Determine if a PROGRAM was supplied or not.
4. Loop through the entries in the ROOT_DIRECTORY:
• if an entry is regular file, check if it contains text matching PATTERN
• if the file does “match,” then either: (1) call PROGRAM passing it the matching
file’s absolute path as its only command-line argument, or (2) if PROGRAM was not
given, print the file’s relative path (relative to ROOT_DIRECTORY).
5. Successful completion of the script should result in an exit status of 0 (zero), which is
the Linux/UNIX standard for successful completion, else a status of 1 for failure.
