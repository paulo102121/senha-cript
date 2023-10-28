#Helper to encrypt strings with custom key with php
composer require senha/cript

use Senha\Cript\SaltCrypt;

$mykey = "mykey";

$secret = "password";

$scp = new SaltCrypt($mykey, $secret);

$encrypted = $scp->encrypt();


$decrypted = $scp->decrypt($mykey);

(It's converted to base_64 in order to save in mysql)

