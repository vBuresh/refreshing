# ReFreshing
**ReFreshing** v3.0.1-alpha2 is a theme for the Hugo with Bootstrap (v5.3). 

>**Внимание!** 
>
>1. Все компоненты этой версии темы **ReFreshing** находятся в стадии активной разработки и могут отображаться с искажениями.
>2. Подробные рекомендации разработчиков Hugo по всем вопросам, связанным с началом работы и применением этого простого и быстрого генератора статических сайтов, приведены в документации Hugo, [на официальном сайте проекта - gohugo.io](https://gohugo.io).

Чтобы создать новый сайт, с условным именем **idealproj**, темой **ReFreshing**, со всеми настройками по умолчанию, которые легко изменить, и демонстрационным наполнением пользовательского каталога *content*, необходимо выполнить следующие команды.

```bash {linenos=table,hl_lines=["4","6-7"],linenostart=1}
hugo new site idealproj && cd idealproj && git init
git submodule add git@github.com:vBuresh/refreshing themes/refreshing
cp -R themes/refreshing/exampleSite/* ./ && mv hugo.toml hugo.toml~
hugo server
```

1. Строка 1 — создать новый сайт, перейти в корневой каталог этого сайта и создать в нем новый Git-репозиторий. 
2. Строка 2 — подключить тему **refreshing** как Git-подмодуль 
3. <sup>[1](#fn_1)</sup> Строка 3 — скопировать из каталога **exampleSite** в корневой каталог сайта примеры информационного наполнения (content), и конфигурационный файл (hugo.yaml), а созданный автоматически файл `hugo.toml`, — переименовать в `hugo.toml~`. Если этого не сделать, то сайт сгенерируется неправильно, о чем будет выведено сообщение. В дальнейшем файл `hugo.toml~` можно уда:лить.
4. Строка 4 — сгенерировать сайт **idealproj**, с темой **ReFreshing**.
---
<sup id="fn_1">1</sup>
При необходимости все действия команд, указанных с строке 3, можно выполнить в любое время. Также можно вручную скопировать файлы в пользовательский каталог `content`, а конфигурационный файл написать самостоятельно, и/или сконвертировать в удобный для пользователя формат (yaml, toml или json).
