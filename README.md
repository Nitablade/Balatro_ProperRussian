# Balatro ProperRussian (by Nitablade)
EN:

This is my own Russian localization for Balatro (game version 1.0.1o-FULL)

RU:
## Краткое описание:
Это моя авторская локализация на русский язык для Balatro (релиз 1.0.1o-FULL)

Для полноценной работы (корректный шрифт, патчи хардкод строк) вам нужна приобретённая копия игры в Steam.

Мод никак не влияет на получение достижений.

## Зачем, если русский язык уже есть в игре?

Официальный перевод оставляет желать много лучшего, а также содержит много ошибок и неточностей. Основные отличия моей локализации:

- Единый стиль написания, везде где это возможно
- Добавлены русифицированные текстуры для всех Джокеров, купонов, карт планет, карт Таро, Спектральных карт, бустерных наборов и прочего
- Вручную добавлена локализация для строк, изначально не поддерживающих перевод
- Исправления некорректных кейвордов по типу "Получает", "Даёт" и т.д.
- Использование буквы "**ё**" в строках
- Дополнительная неочевидная информация в описании некоторых карт, имеющаяся только на офф. Вики игры
- Локализация не следует точь-в-точь написанию в английской версии, а призвана быть максимально простой и хорошо читаемой

В моде также заменён шрифт на доработанный **Mini Pixel 7**, не стремясь повторить оригинальный, но пиксельный, хорошо читабельный и вписывающийся в сеттинг. Альтернативный шрифт, копирующий англоязычный **m6x11plus** лежит в папке ```/extra```.

## Как установить (на Windows):
Подробный гайд на странице [Releases](https://github.com/Nitablade/Balatro_ProperRussian/releases)

Если не сложно, оставьте какую-нибудь реакцию и/или комментарий под этим постом для продвижения: (сначала присоединитесь к [офф. серверу Balatro](https://discord.gg/cbbuVAU9)): [https://discord.com/channels/1116389027176787968/1217140107962748949/1217140107962748949](https://discord.com/channels/1116389027176787968/1217140107962748949/1217140107962748949)

Спасибо.

## Как установить (на SteamDeck):
Установка происходит точно так же, как на Windows, отличаются только пути для распаковки файлов. А именно, .dll файл:
- Если игра установлена на SD-карте: ```primary/steamapps/common/Balatro```
- Если игра установлена во Внутренней памяти: ```Home/.steam/steam/steamapps/common/Balatro```  
Папка **Appdata** находится по пути: ```Home/.steam/steam/steamapps/compatdata/2379780/pfx/drive_c/users/steamuser/AppData/Roaming/Balatro```

Ещё нужно добавить в ```Steam → Balatro → Свойства → Общие → "Параметры запуска"``` строку: 
**WINEDLLOVERRIDES="version=n,b" %command%**

## Как установить (на Mac):
- Файлы из архива распаковать по пути: ```/Users/Пользователь/Library/Application Support/Balatro```

- [С офф. страницы Lovely-инжектора](https://github.com/ethangreen-dev/lovely-injector/releases) скачать последний релиз для Mac, файлы ```liblovely.dylib``` и ```run_lovely.sh``` закинуть в папку с игрой, запустить игру через ```run_lovely.sh```.

[Подробная инструкция на английском](https://github.com/ethangreen-dev/lovely-injector?tab=readme-ov-file#mac)

## Файловая структура мода:
- ```version.dll``` : Lovely-инжектор, скачивается отдельно с офф. страницы (необходим для применения написанных вручную патчей интерфейса, а также корректных параметров для шрифта)
- ```/mods/ProperRussian/lovely.toml``` : файл, содержащий все вручную написанные патчи, которые применяются поверх игры, не трогая код приложения и не влияя на получение достижений (к каждому патчу присутствует комментарий)
- ```/resources/textures/``` : папка содержит заменяемые игровые текстуры, которые хранятся в файлах ```BlindChips, Boosters, Jokers, ShopSignAnimations, Tarots и Vouchers``` (если хотите играть без них - просто удалите ненужные вам из папки ```/1x``` и ```/2x```)
- ```/resources/fonts/NotoSans-Bold.ttf``` : файл кастомного шрифта, заменяет основной шрифт, использующийся в оф. переводе (не влияет на английский шрифт, если вы захотите поиграть с ним), при желании можно заменить на любой другой шрифт, сохранив такое же название шрифта, а также заменив файл ```lovely.toml``` из папки ```/extra```
- ```/localization/ru.lua``` : файл перевода всех строк, использующихся в игре, в отличие от оф. релиза все строки отсортированы в том же порядке, что и в оригинальном ```en-us.lua```
- ```/extra``` : папка с необязательными к установке элементами, на данный момент содержит альтернативный шрифт и русифицированные текстуры для игральных карт

**Дополнительные опции / Как заменить отдельные элементы:**

Начиная с версии мода **1.0.5**, дополнительный шрифт и другие необязательные к установке опции перенесены в папку ```/extra```. Для их активации просто замените существующие файлы. На данный момент доступны следующие экстра-элементы:
- альтернативный шрифт (копирует стиль оригинального **m6x11plus**)
- русифицированные литеры для игральных карт (В - Валет, Д - Дама, К - Король, Т - Туз) для обычного и высококонтрастного режима
- русифицированные литеры для карт из коллабораций для обычного и высококонтрастного режима

## Известные недочёты:
- В списке правил для испытания *Жестокость*, строка о Блайндах без наград отображается дважды

## Ниже немного скриншотов
![20240327181037_1](https://github.com/Nitablade/Balatro_ProperRussian/assets/109508685/749be51a-b923-4833-909f-ae2f6607dafb)
![20240327181053_1](https://github.com/Nitablade/Balatro_ProperRussian/assets/109508685/f42e2473-44a9-42c3-83ce-ac0c292c0ab0)
![20240327181107_1](https://github.com/Nitablade/Balatro_ProperRussian/assets/109508685/ba86b08e-e3dc-4fa1-895a-784e33dd32e8)
![20240412044015_1](https://github.com/Nitablade/Balatro_ProperRussian/assets/109508685/d0c9fda3-6549-436d-abbd-0533c801d2d5)
![20240327181211_1](https://github.com/Nitablade/Balatro_ProperRussian/assets/109508685/29c19d05-456c-4ce9-94bc-d9c7133fcd76)
![20240327181234_1](https://github.com/Nitablade/Balatro_ProperRussian/assets/109508685/d48b1cdf-ddbc-4f5f-b838-fc087bc46b6a)
![20240327181314_1](https://github.com/Nitablade/Balatro_ProperRussian/assets/109508685/23ee7f4a-21c3-40d2-a853-b5438f2c7f91)

### Выразить благодарность автору локализации можно тут: [https://www.twitch.tv/Nitablade](https://www.twitch.tv/Nitablade)

Помимо Balatro, я занималась локализацией для таких игр как:
1) [**BEAM**](https://store.steampowered.com/app/1067430/Beam/)
2) [**Backpack Hero**](https://store.steampowered.com/app/1970580/Backpack_Hero/)
3) [**Мод Downfall**](https://steamcommunity.com/sharedfiles/filedetails/?id=1610056683&searchtext=Downfall) для Slay the Spire
4) [**Wildfrost**](https://github.com/Nitablade/Wildfrost_RU)

Также можете присоединиться к моему [Discord-серверу](https://discord.gg/zFAGDn6QMs), чтобы следить за обновлениями локализаций.
