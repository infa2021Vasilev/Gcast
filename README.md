# Gcast

**Требования к программному обеспечению**

Программа Python v 3.8.5

Библиотеки:

- pygame v 2.0.2.
- random
- math
- os
- sys
- threading
- cv2
- moviepy.editor
- time
- colorama

**Управление**

**Внутри игры**** :**

**W**** , **** S ****,**  **D**** , **** A **** – **Движение** вперёд, назад, вправо, влево** соответственно

**1, 2, 3 –** Выбор оружия

**Mouse** – поворот персонажа и прицеливание, в том числе по вертикали (попадания в голову врага наносят больше урона)

**ESC**  **–** вызов меню: RESUME – возобновить игру, MAINMENU – вернуться в главное меню, QUIT – выйти из игры

**В главном меню:**

SINGLEPLAYER – Запустить одиночную игру, MULTIPLAYER – Запустить меню сетевой игры: CREATESERVER – Меню создания сервера: ENTERPORT – Поле ввода порта, CREATESERVER – Запускает игру, открытую для другого игрока, BACK – Вернуться в главное меню; JOINSERVER – меню присоединения к другому серверу: ENTERPORT – Поле ввода порта, ENTERIP – Поле ввода IP сервера, на котором игрок собирается играть, JOINSERVER – Присоединиться к сетевой игре на удалённом сервере, BACK – Вернуться в главное меню

**Описание внутриигровых объектов**

Враг – существует 3 типа, они отличаются анимациями и звуками, к ним нельзя подойти ближе чем на одну клетку, увидев игрока враг начнёт стрелять и приближаться к игроку, нанося урон, получив достаточное количество урона, враг погибнет с характерной анимацией смерти.

**Процесс игры**

При запуске игры проигрывается вступительный ролик с звуковой дорожкой (при нажатии ESC ролик будет пропущен)

**В игре присутствует сетевая и одиночная игра:**

-Чтобы победить в одиночной игре необходимо пройти автоматически сгенерированный лабиринт, попутно уничтожая препятствия (врагов), при этом не допустив потери всех 100 жизней (в этом случае игра будет проиграна и игрока вернёт в главное меню). В случае успешного прохождения лабиринта игроку будет показан финальный синематик с титрами и звуковой дорожкой (при нажатии ESC ролик будет пропущен).

-Чтобы победить в сетевой игре, необходимо уничтожить игрока противника (в игре), проигравший будет возвращён в главное меню, чтобы сыграть следующий матч необходимо перезапустить игровую сессию.
