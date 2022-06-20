На входе у нас два файла и описание cipher.txt, private.pem. Описание гласит "А вы ноктюрн сыграть могли бы на флейте водосточных труб(Кириллица)" это отсылает нас к стихотворению Маяковского.


Расшифруем через openssl 

openssl rsautl -in cipher.txt -inkey private.pem -out decipher.txt -decrypt


Нас просят ввести passphrase: исходя из условия введем кириллицой mayakovskiy.

В файле decipher.txt получаем флаг KVVUCTF{R$A_$nD_D3S_w4S_eAsY}
