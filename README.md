# DiskSpaceParser
Really cheap and nasty KIXtart script to connect to a list of shares and grab the free space on them.

This small KiXtart app creates a file with the free space available on shares in an input file
By Neil Holmes 18/02/2010

IMPORTANT: This script will unmap your X: drive. If you have a share on that drive, search for X: in Disk space parse.kix and amend it to a free drive letter

To use this, you'll need to copy it locally to your PC, it doesn't matter where or on which local drive.

To use:

1. Generate the names of the shares you want to check the free space on
2. Put the share names into a file called servers.txt, one share per line. For example
\\d-ap1\c$
\\d-ap2\c$
Any additional lines that don't match the syntax of a UNC path will be echoed in the output file
3. Make sure the files Disk space parse.kix, KIX32.EXE and RUNME.bat are on one of your local disks and in the same directory
4. Double click RUNME.bat
5. Wait for the script to complete, then a file called output.csv will be generated containing the free space on all the shares in servers.txt
6. Profit
