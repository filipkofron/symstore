# symstore

A python module and command lite utility for publishing windows debugging symbols to 
symbols store. The symbols published in this format can be consumed by the common
development tools for windows, such as Visual Studio and WinDbg. See 
[Using SymStore](https://msdn.microsoft.com/en-us/library/windows/desktop/ms681417%28v=vs.85%29.aspx)
for more information on windows symbols store.

Currently it is possible to publish PDB and PE (exe and dll) files to a local file 
system.

## Installing

This package can be installed with pip utility. 
You need to clone this repository:

    $ git clone <repo-url> symstore

and install it with pip:

    $ pip install symstore/

This will install the command line utility 'symstore' as well as python module 
'symstore'.

## Using

### command line

Use the 'symstore' command to publish the symbols. Run 'symstore --help' for 
details.

### Python module

To publish symbols programmatically use the 'symstore' module. See symstore/bin/symstore for an example on how to use the API.