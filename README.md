# resetting_network
Как посмотреть IP адрес. С помощью командной строки.
Открываем консоль cmd.
![image](https://github.com/tvgVita69/resetting_network/assets/98489171/3c023254-0faa-4920-8f7b-3c65f339c635)
 
Далее пишем команду ipconfig /all
 
Или через powershell. 
![image](https://github.com/tvgVita69/resetting_network/assets/98489171/a686c08a-dd22-49af-aaf9-b010d624d85a)
![image](https://github.com/tvgVita69/resetting_network/assets/98489171/8d988836-bbb9-46c0-b078-0103650c49c4)
![image](https://github.com/tvgVita69/resetting_network/assets/98489171/8c8369a0-c874-44eb-93be-ade0b276ad4d)
 
 
Чтобы посмотреть какие еще есть команды, набираем ipconfig /?
![image](https://github.com/tvgVita69/resetting_network/assets/98489171/f5089add-8093-4c0e-bc7e-1de4fa3143c5)
 
Есть еще одна команда для продвинутых пользователей, через которую можно посмотреть настройки, статистику и другую информацию. С помощью этой команды, так же можно корректировать некоторые сетевые настройки.  Это команда netsh /?
![image](https://github.com/tvgVita69/resetting_network/assets/98489171/23a07a95-dc89-4d81-90c1-949065633a8d)

 
Например, если хотите посмотреть IP адреса, то можно прописать так
netsh int ip show config или  netsh int ip show addresses
![image](https://github.com/tvgVita69/resetting_network/assets/98489171/eac3a953-d93f-4812-8f9f-d3ca7d02e4ad)
 
Если не удается подключиться к Интернету, можно сбросить параметры протокола TCP/IP и восстановить исходное состояние TCP/IP. Команда вступает в силу после перезагрузки компьютера.
netsh int ip reset 
Или команда, которая сбрасывает настройки Winsock и восстанавливает ваш компьютер после любых ошибок сокетов. Winsock содержит настройки подключения вашего компьютера к Интернету.
netsh winsock reset

Как посмотреть IP адрес на машине с OS Linux, например Ubuntu.
В отличии от OS Windows в этих системах обширный набор команд.
Для просмотра IP адреса используют команду ip a или ifconfig.
![image](https://github.com/tvgVita69/resetting_network/assets/98489171/304aae1f-15ef-497d-abfc-8c2ed0b5b23e)
  
Если более точнее, например убрать всё лишнее.
![image](https://github.com/tvgVita69/resetting_network/assets/98489171/4a796130-cce6-4fc8-a554-0d55dcba29ac)
 
Полный мануал по ним, можно посмотреть так ip –help или ifconfig –help.
![image](https://github.com/tvgVita69/resetting_network/assets/98489171/d3385783-b9b8-40c3-a11e-174ccb3298d6)
 
Как узнать внешний адрес.
wget -qO- ipecho.net или так wget -qO- ident.me
Такой конструкцией wget -qO- ipecho.net можно вывести в веб браузере 
![image](https://github.com/tvgVita69/resetting_network/assets/98489171/288fb4ef-5c4c-4a9c-bde0-c6086a245182)
 


