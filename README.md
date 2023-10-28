# Helper to encrypt strings with custom key with php

[![Unit Tests](https://github.com/fruitcake/php-cors/actions/workflows/run-tests.yml/badge.svg)](https://github.com/fruitcake/php-cors/actions)
[![PHPStan Level 9](https://img.shields.io/badge/PHPStan-Level%209-blue)](https://github.com/fruitcake/php-cors/actions)
[![Code Coverage](https://img.shields.io/badge/CodeCoverage-100%25-brightgreen)](https://github.com/fruitcake/php-cors/actions/workflows/run-coverage.yml)
[![Packagist License](https://poser.pugx.org/fruitcake/php-cors/license.png)](http://choosealicense.com/licenses/mit/)
[![Latest Stable Version](https://poser.pugx.org/fruitcake/php-cors/version.png)](https://packagist.org/packages/fruitcake/php-cors)
[![Total Downloads](https://poser.pugx.org/fruitcake/php-cors/d/total.png)](https://packagist.org/packages/fruitcake/php-cors)
[![Fruitcake](https://img.shields.io/badge/Powered%20By-Fruitcake-b2bc35.svg)](https://fruitcake.nl/)

Library and middleware enabling cross-origin resource sharing for your
http-{foundation,kernel} using application. It attempts to implement the
[W3C Recommendation] for cross-origin resource sharing.

[W3C Recommendation]: http://www.w3.org/TR/cors/

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





