# Домашнее задание: «Защита хоста»

## Задание 1

Установил eCryptfs и создал пользователя `cryptouser`.  
Домашний каталог был успешно зашифрован.

### Скриншоты
1. Вид под пользователем `cryptouser` (читаемые файлы):  
![](screenshot/cryptouser_home.png)

2. Вид из-под root в `/home/.ecryptfs/cryptouser/.Private` (зашифрованные имена):  
![](screenshot/encrypted_private.png)

## Задание 2

Установил поддержку `LUKS`, создал раздел 100 Мб и зашифровал его с помощью `cryptsetup`.

### Скриншоты
1. Установка cryptsetup и проверка версии:  
![](screenshot/hw_2.1.png)

2. Создание виртуального раздела 100 Мб:  
![](screenshot/hw_2.2.png)

3. Инициализация LUKS (`luksFormat`):  
![](screenshot/hw_2.3.png)

4. Открытие раздела и создание файловой системы ext4:  
![](screenshot/hw_2.4.png)

5. Монтирование и проверка содержимого (`lost+found`):  
![](screenshot/hw_2.5.png)

6. Размонтирование и закрытие раздела:  
![](screenshot/hw_2.6.png)
