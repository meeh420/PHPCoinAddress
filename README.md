PHPCoinAddress
==============

PHPCoinAddress is a PHP object that creates public/private address key pairs for 
Bitcoin, Namecoin, Litecoin, PPCoin, Devcoin, and other cyrptocoins.

Version 0.1.7

* Info: https://github.com/zamgo/PHPCoinAddress
* Download ZIP: https://github.com/zamgo/PHPCoinAddress/archive/master.zip
* Git clone: https://github.com/zamgo/PHPCoinAddress.git


Usage:
==============
<pre>
require_once 'PHPCoinAddress.php'; 
// CoinAddress::set_debug(true);      // optional - show debugging messages 
// CoinAddress::set_reuse_keys(true); // optional - use same key for all addresses 
$coin = CoinAddress::bitcoin();  
print "\nBITCOIN: (uncompressed)\n";
print 'public: ' . $coin['public'] . "\n";
print 'public (Hexadecimal): ' . $coin['public_hex'] . "\n";
print 'private (Wallet Import Format): ' . $coin['private'] . "\n";
print 'private (Hexadecimal): ' . $coin['private_hex'] . "\n"; 
</pre>

Notes:
==============
- modded from https://gist.github.com/scintill/3549107
- includes elliptic curve cryptography (ECC) libraries from https://github.com/mdanter/phpecc
- requires PHP extension BCMATH or GMP.  (GMP is much faster)

License:
==============
Copyright (C) 2013 PHPCoinAddress Developers

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the "Software"),
to deal in the Software without restriction, including without limitation
the rights to use, copy, modify, merge, publish, distribute, sublicense,
and/or sell copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included
in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

