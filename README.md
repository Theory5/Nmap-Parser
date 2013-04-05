Nmap-Parser
=================================================================

Parse nmap scan data with perl

This module implements a interface to the information contained in an nmap scan. It is implemented by parsing the xml scan data that is generated by nmap. This will enable anyone who utilizes nmap to quickly create fast and robust security scripts that utilize the powerful port scanning abilities of nmap.

Installation
=================================================================

* Latest version: [https://github.com/apersaud/Nmap-Parser](https://github.com/apersaud/Nmap-Parser)

Manual Install
=================================================================

Download the file and unpack. This is usually done by:

    tar zxvf Nmap-Parser-x.xx.tar.gz

Where x.xx is the version number. Next change into the newly created directory. To install this module type the following:

    perl Makefile.PL
    make
    make test
    make install

If you would like to install Nmap-Parser in a different directory (or if you do
not have root access use `perl Makefile.PL PREFIX=/install/path`, where
`/install/path` is the directory in which you want to install the module. Note
that you should then use the "use lib '/install/path'" in your scripts.


ActiveState Perl (Perl Package Manager) - MSWin32
=================================================================

Run this in the command prompt:

    ppm install Nmap-Parser

This should contact the ActiveState respository, download the file and install it automagically.

CPAN Install (If you are missing dependencies)
=================================================================

Run this in the command prompt to install directly from CPAN (may need root priviledges):

	perl -MCPAN -e 'install Nmap::Parser'
	

Dependencies
=================================================================

This module requires these other modules and libraries:

* XML::Twig 3.16+
* Storable (comes with Perl 5+)
	

In addition, you will need nmap 3.00+. You don't exactly need it, but this
version of nmap supports the xml output that this module can parse. So, you do
not really need the executable, but the xml output that you will be parsing
(or able to parse), must be from this version onward.

Copyright and License
=================================================================

Copyright (C) 2003-2011 Anthony Persaud L<http://modernistik.com>

MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

