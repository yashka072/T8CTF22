У нас есть два файла cipher.txt, private.pem заходим в openssl и попытаемся расшифровать через сервис rsautl



openssl rsautl -in cipher.txt -inkey private.pem -out decipher.txt -decrypt.
В файле decipher.txt видим флаг
KVVUCTF{eA$y_R$A_4_Y0u}
