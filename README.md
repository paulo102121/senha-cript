Helper to encrypt strings with custom key with php

In composer

composer require master102121/encryptor

use Senha\Cript\SaltCrypt;

$mykey = "mykey";

$secret = "password";

$scp = new SaltCrypt($mykey, $secret);

$encrypted = $scp->encrypt();


$decrypted = $scp->decrypt($mykey);

