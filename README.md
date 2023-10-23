# yandex-translator
тест-кейсы для яндекс переводчика (тестовое задание)

<img src="https://sun9-49.userapi.com/impg/VGE0qumLcfz-Hyd1n9TLGrvrLEdVRy-oRYuChg/a_lGB-0fxFs.jpg?size=637x500&quality=96&sign=6abaef7d083af84742ade48c75731d0f&type=album" height="450">

### Тест-кейсы:

| №  | Название                        | Предусловия                           | Тестовые данные     | № шага | Шаги                                                    | Ожидаемый результат                                                                                      |
|----|-----------------------------------------------|------------------------------------------------------|---------------------|--------|---------------------------------------------------------|----------------------------------------------------------------------------------------------------------|
| 1  | Переход на полную версию переводчика                                                        | |                     | 1      | Нажать на ссылку "Словарь и онлайн перевод..."          | Осуществился переход на страницу https://translate.yandex.ru/                                            |
| 2  | Проверка выбора языка ввода                                                                 |                                                                                                                                                                  |                     | 1      | Нажать на кнопку выбора языка                           | Открылся выпадающий список                                                                               |
|    |                                                                                             |                                                                                                                                                                  |                     | 2      | Пролистать до нужного языка                             | Список скроллится, полоса прокрутки не перекрывает текст                                                 |
|    |                                                                                             |                                                                                                                                                                  |                     | 3      | Выбрать любой язык                                      | Выпадающий список закрылся, язык отобразился над полем ввода текста                                      |
| 3  | Проверка выбора языка перевода                                                              |                                                                                                                                                                  |                     | 1      | Нажать на кнопку выбора языка                           | Открылся выпадающий список                                                                               |
|    |                                                                                             |                                                                                                                                                                  |                     | 2      | Пролистать до нужного языка                             | Список скроллится, полоса прокрутки не перекрывает текст                                                 |
|    |                                                                                             |                                                                                                                                                                  |                     | 3      | Выбрать любой язык                                      | Выпадающий список закрылся, язык отобразился над полем ввода текста                                      |
| 4  | Проверка корректности перевода тестовых данных на английский                                |                                                                                                                                                                  | кошка, собака, тест | 1      | Выбрать язык ввода Русский                              | Над полем ввода текста отображается "Русский"                                                            |
|    |                                                                                             |                                                                                                                                                                  |                     | 2      | Выбрать язык перевода Английский                        | Над полем перевода текста отображается "Английский"                                                      |
|    |                                                                                             |                                                                                                                                                                  |                     | 3      | Ввести тестовые данные в поле ввода                     | В поле ввода пропадает плейсхолдер "Введите текст" и отображается введённый текст                        |
|    |                                                                                             |                                                                                                                                                                  |                     | 4      | Проверить переведённый текст                            | В переводе отобразилось "cat, dog, test"                                                                 |
| 5  | Проверка корректности перевода тестовых данных на русский                                   |                                                                                                                                                                  | сat, dog, test      | 1      | Выбрать язык ввода Английский                           | Над полем ввода текста отображается "Английский"                                                         |
|    |                                                                                             |                                                                                                                                                                  |                     | 2      | Выбрать язык перевода Русский                           | Над полем перевода текста отображается "Русский"                                                         |
|    |                                                                                             |                                                                                                                                                                  |                     | 3      | Ввести тестовые данные в поле ввода                     | В поле ввода пропадает плейсхолдер "Введите текст" и отображается введённый текст                        |
|    |                                                                                             |                                                                                                                                                                  |                     | 4      | Проверить переведённый текст                            | В переводе отобразилось "кошка, собака, тест"                                                            |
| 6  | Проверка корректности перевода при нажатии на кнопку "обратный перевод"                     |                                                                                                                                                                  | кошка, собака, тест | 1      | Выбрать язык ввода Русский                              | Над полем ввода текста отображается "Русский"                                                            |
|    |                                                                                             |                                                                                                                                                                  |                     | 2      | Выбрать язык перевода Английский                        | Над полем перевода текста отображается "Английский"                                                      |
|    |                                                                                             |                                                                                                                                                                  |                     | 3      | Ввести тестовые данные в поле ввода                     | В поле ввода пропадает плейсхолдер "Введите текст" и отображается введённый текст                        |
|    |                                                                                             |                                                                                                                                                                  |                     | 4      | Проверить переведённый текст                            | В переводе отобразилось "cat, dog, test"                                                                 |
|    |                                                                                             |                                                                                                                                                                  |                     | 5      | Нажать на кнопку обратный перевод                       | языки ввода и перевода поменялись местами, осуществлён обратный перевод (в переводе кошка, собака, тест) |
| 7  | Проверка корректности автоматического определения языка при вводе текста                    |                                                                                                                                                                  | cat                 | 1      | Выбрать язык ввода Русский                              | Над полем ввода текста отображается "Русский"                                                            |
|    |                                                                                             |                                                                                                                                                                  |                     | 2      | Ввести тестовые данные в поле ввода                     | Над полем ввода текста язык сменяется на "Английский (определено)"                                       |
| 8  | Проверка удаления введенного текста нажатием на кнопку крестика (очистить) в поле ввода     |                                                                                                                                                                  | тест                | 1      | Ввести тестовые данные в поле ввода                     | Кнопка вставки текста меняется на кнопку очистки в виде крестика                                         |
|    |                                                                                             |                                                                                                                                                                  |                     | 2      | Нажать на крестик                                       | Текст удалён                                                                                             |
| 9  | Проверка копирования текста из буфера обмена нажатием на кнопку вставки текста в поле ввода | 1) Скопировать любой текст                                                                                                                                       |                     | 1      | Нажать на кнопку вставки текста в поле ввода            | Скопированный ранее текст вставлен                                                                       |
| 10 | Проверка корректности ввода текста с помощью голосового ввода                               |                                                                                                                                                                  | кошка, собака, тест | 1      | Выбрать язык ввода Русский                              | Над полем ввода текста отображается "Русский"                                                            |
|    |                                                                                             |                                                                                                                                                                  |                     | 2      | Нажать на кнопку микрофона (ввести голосом)             | На кнопке появляется анимация на время ввода                                                             |
|    |                                                                                             |                                                                                                                                                                  |                     | 3      | Назвать тестовые данные                                 | Тестовые данные распознаны и отображаются корректно в поле ввода                                         |
| 11 | Проверка корректности голосового вывода введенного текста                                   |                                                                                                                                                                  | кошка, собака, тест | 1      | Ввести тестовые данные в поле ввода                     | В поле ввода пропадает плейсхолдер "Введите текст" и отображается введённый текст                        |
|    |                                                                                             |                                                                                                                                                                  |                     | 2      | Нажать на кнопку голосового вывода введенного текста    | Текст озвучен корректно                                                                                  |
| 12 | Проверка копирования переведённого текста нажатием на кнопку копирования в поле перевода    |                                                                                                                                                                  | кошка, собака, тест | 1      | Выбрать язык ввода Русский                              | Над полем ввода текста отображается "Русский"                                                            |
|    |                                                                                             |                                                                                                                                                                  |                     | 2      | Выбрать язык перевода Английский                        | Над полем перевода текста отображается "Английский"                                                      |
|    |                                                                                             |                                                                                                                                                                  |                     | 3      | Ввести тестовые данные в поле ввода                     | В поле ввода пропадает плейсхолдер "Введите текст" и отображается введённый текст                        |
|    |                                                                                             |                                                                                                                                                                  |                     | 4      | Проверить переведённый текст                            | В переводе отобразилось "cat, dog, test"                                                                 |
|    |                                                                                             |                                                                                                                                                                  |                     | 5      | Нажать на кнопку копирования текста в поле перевода     | Появляется текст "Перевод скопирован"                                                                    |
|    |                                                                                             |                                                                                                                                                                  |                     | 6      | Вставить текст в текстовый редактор                     | Вставлен текст "cat, dog, test"                                                                          |
| 13 | Проверка корректности голосового вывода переведённого текста                                |                                                                                                                                                                  | кошка, собака, тест | 1      | Выбрать язык ввода Русский                              | Над полем ввода текста отображается "Русский"                                                            |
|    |                                                                                             |                                                                                                                                                                  |                     | 2      | Выбрать язык перевода Английский                        | Над полем перевода текста отображается "Английский"                                                      |
|    |                                                                                             |                                                                                                                                                                  |                     | 3      | Ввести тестовые данные в поле ввода                     | В поле ввода пропадает плейсхолдер "Введите текст" и отображается введённый текст                        |
|    |                                                                                             |                                                                                                                                                                  |                     | 4      | Проверить переведённый текст                            | В переводе отобразилось "cat, dog, test"                                                                 |
|    |                                                                                             |                                                                                                                                                                  |                     | 5      | Нажать на кнопку голосового вывода переведённого текста | Перевод озвучен корректно                                                                                |
