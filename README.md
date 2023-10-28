# Helper to encrypt strings with custom key with php

[![Latest Stable Version](http://poser.pugx.org/senha/cript/v)](https://packagist.org/packages/senha/cript) [![Total Downloads](http://poser.pugx.org/senha/cript/downloads)](https://packagist.org/packages/senha/cript) [![Latest Unstable Version](http://poser.pugx.org/senha/cript/v/unstable)](https://packagist.org/packages/senha/cript) [![License](http://poser.pugx.org/senha/cript/license)](https://packagist.org/packages/senha/cript) [![PHP Version Require](http://poser.pugx.org/senha/cript/require/php)](https://packagist.org/packages/senha/cript)


> Note: It's converted to base_64 in order to save in mysql
## Installation

composer require senha/cript

## Usage

use Senha\Cript\SaltCrypt;

$mykey = "mykey";

$secret = "password";

$scp = new SaltCrypt($mykey, $secret);

$encrypted = $scp->encrypt();

$decrypted = $scp->decrypt($mykey);

Output:lHi57dDf8qNWmhbq8M2s82TMplWWU9Yqr0BQptZCzik5p6y5yHzXR4E0SLJVJaBcgrUf7NjZsG+SEw==




