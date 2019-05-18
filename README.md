# maze
## Описание

Небольшая консольная игра, цель которой - дойти до заданной точки в темном лабиринте. Игрок видит 
только на определенный радиус вокруг себя, остальная часть лабиринта находится в тени и не различима.

На начальном экране можно выбрать настройки игры:
* Символы, которыми будет отрисовываться лабиринт - только ascii символы или unicode, 
 позволяющий отображать стены более красиво.
* Ширину экрана - для того, чтобы картинка влезала в терминал и смотрелась правильно.
* Радиус, на котором игрок видит лабиринт. Влияет на сложность игры.

> Рис 1. Меню Настроек

    Welcome to the MAZE game. The goal of the game is reaching the target in the dark labyrinth.
    Player is able to see some area around himself. Good luck.

    Select mode:
     - (u)nicode for regular characters
     - (a)scii for ASCII-only characters
    > u

    Enter terminal width in characters (120 is recommended, 40 is minimal)
    > 40 

    Enter the radius of circle player is able to see (3 for hard, 5 for medium, > 7 for easy)
    > 3


После выбора настроек появляется лабиринт. Перемещаться в нем можно, вводя команды. Переместиться на 
одну клетку можно с помощью команд w/a/s/d или u/l/b/r. Введя букву два раза, можно переместиться до
ближайшей стены.

> Рис 2. Лабиринт

    **************************************                              
    ************************************** Movement                     
    ******************************  ******   t/w - Top, r/d - Right,    
    **************************  ║       **   b/s - Bottom, l/a - Left   
    **************************  ╚═══╗   **                              
    ************************║     A ║   ║  Enter letter twice to move   
    **************************══╗   ║   ** up to the wall.              
    **************************  ║   ║   **                              
    ******************************  ******                              
    ************************************** Legend                       
    **************************************   A  - Player                
    **************************************   ╔═ - Wall                  
    **************************************   ** - Shadow                
    **************************************   }{ - Objective             
    **************************************                              
    **************************************                              
    **************************************
    **************************************
    **************************************
    **********************************}{**
    **************************************
    > s

## Запуск
Из корневой директории проекта `java -jar maze`.

## Схема классов
Доступна по ссылке https://drive.google.com/file/d/1idQI0lfpe_ykAT_yNoXbSKc4-uvhI9Eh/view?usp=sharing
