Схема
===
Клиент вводит свои данные при регистрации ИНН и снилс. Сервер создает хэш и проверяет его на уникальность в базе
Если подобный хэш есть - клиент зареган, иначе - выдаем ему хэш. параллельно генерятся 2 ассиметричных ключа A(1,2)
 и B(1,2)
Есть несколько путей развития системы:

1)Клиент хочет провести транзакцию-перевести средства кому-то. создается транзакция в которой указывается получатель, 
суммма итд... и вс это шифруется ключем A1. Ядро расшифровывает это сообщение с пом А2 и принимает какое-то решение. 
Результат своего решения шифрует ключем В1 и отправляет клиету, который расшифровывает это сообщение ключем В2

..............
