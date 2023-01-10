[Bash-скрипт](https://github.com/eugrus/PermArch/blob/main/script), который скачивает изображения всех листов дела с сайта [Государственного архива Пермского края](https://archives.permkrai.ru) и собирает из них PDF.

Для работы скриптом в системе должны быть установлены `img2pdf` и `wget`.

Перед работой со скриптом нужно залогиниться на сайте https://archives.permkrai.ru и экспортировать куки от этого сайта в размещаемый в каталоге со скриптом файл `archives.permkrai.ru_cookies.txt`. Для экспорта куки можно воспользоваться расширением <em>Chrome</em> [<em>Get cookies.txt</em>
](https://chrome.google.com/webstore/detail/get-cookiestxt/bgaddhkoddajcdgocldbbfleckgcbcid). Если куки-файл в каталоге устарел, то полученные изображения окажутся пустыми.

Первым параметром скрипту нужно предоставить ID дела на сайте, а вторым количество листов в деле.

К примеру, в случае https://archives.permkrai.ru/archive1/unit/956780 вызов скрипта нужен такой:

`./script 956780 118`

Тогда на выходе будет получен файл `956780.pdf` в каталоге со скриптом.
