
Hashids Spark for CodeIgniter
============================

A [CodeIgniter](http://codeigniter.com) [Spark](http://getsparks.org/) for implementing [Hashids](http://www.hashids.org) to generate hashes (like YouTube or Bitly) from numbers to obfuscate database IDs.


Installation
-------------------------------------

1. Install the spark: `php tools/spark install sk-hashids` - or, if not using Spark package management, copy `hashids_helper.php` to your `application/helpers` folder & `config/hashids.php` to your `application/config` folder.
2. Load the spark: `$this->load->spark('sk-hashids/1.0.5');` - or, optionally autoload the spark in `application/config/autoload.php`: $autoload['sparks'] = array('sk-hashids/1.0.5');`.
3. Employ helper functions as needed.


Usage
-------------------------------------

	Encrypt: <?=hashids_encrypt(1234)?>
	Decrypt: <?=hashids_decrypt("1lj")?>

	Custom Encrypt: <?=hashids_encrypt(1234, 'alternate config salt', 10)?>
	Custom Encrypt: <?=hashids_decrypt('pjxalngQJ3', 'alternate config salt', 10)?>


License
-------------------------------------

Copyright © 2013 Jason M Horwitz, Sekati LLC. All Rights Reserved.

Released under the MIT License: [http://www.opensource.org/licenses/mit-license.php](http://www.opensource.org/licenses/mit-license.php)

	The MIT License

	Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
	associated documentation files (the “Software”), to deal in the Software without restriction,
	including without limitation the rights to use, copy, modify, merge, publish, distribute,
	sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is
	furnished to do so, subject to the following conditions:

	The above copyright notice and this permission notice shall be included in all copies or
	substantial portions of the Software.

	THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING
	BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
	NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
	DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
	OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
