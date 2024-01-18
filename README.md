# eblanokod

Фрагменты уязвимого кода с комментариями

## Скрытие пароля

ну, конечно, если каким-то алгоритмом типа base64 зашифровать пароль, то никто его "точно не узнает":

```php
    $mail->Username = 'email европедораса'; // SMTP username
    $mail->Password = Crypto::decrypt(
		hex2bin('8e0116c0f7662b394156632cdb628afb2a5add96bf7bba88'), 
		hex2bin('566f6c6f73506f7274417574686f726974795f323032335f')
	); // SMTP password
```
