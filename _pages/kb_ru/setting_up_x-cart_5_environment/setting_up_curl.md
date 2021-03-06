---
lang: ru
layout: article_with_sidebar
updated_at: '2017-11-21 12:38 +0400'
identifier: ref_7acvbbTA
title: Настройка cURL
order: 30
published: true
---

[cURL](http://php.net/manual/ru/intro.curl.php) - это PHP расширение, которое устанавливает соединение с различными видами серверов. X-Cart использует cURL для подключения к маркетплейсу и установки из него модулей. Обычно, хостинг провайдеры компилируют PHP для работы с cURL, и все отлично работает. Если это не ваш случай - эта статья для вас. 

Некорректная настройка PHP и cURL может вызвать ряд проблем, решение которых описывает данная статья.

## Содержание

*   [cURL не работает на сервере](#curl-не-работает-на-сервере)
*   [cURL не работает на локальном компьютере](#curl-не-работает-на-локальном-компьютере)
    *   [Windows + XAMPP](#windows--xampp)
    *   [Ubuntu/Debian + Apache](#ubuntudebian--apache)
    
## cURL не работает на сервере

Обычно, для решения этой проблемы достаточно попросить хостинг провайдера [скомпиллировать PHP с cURL](http://php.net/manual/ru/curl.installation.php). Но прежде чем обращаться в поддержку хостинга, проверьте, есть ли в вашей панели управления на хостинге возможность активировать cURL. Если у вас выделенный сервер и вы можете самостоятельно управлять расширениями, прочтите инструкции ниже.

## cURL не работает на локальном компьютере

В этом случае, решение зависит от того, какие у вас сервер и операционная система.

### Windows + XAMPP

1. Найдите эти три файла на своем компьютере:

  - `C:\Program Files\xampp\apache\bin\php.ini`
  - `C:\Program Files\xampp\php\php.ini`
  - `C:\Program Files\xampp\php\php4\php.ini`

2. В каждом из них замените эту часть кода:

   ```
   ;extension=php_curl.dll
   ```
    
   на этот код:
    
   ```
   extension=php_curl.dll
   ```

3. Перезапустите Apache.

### Ubuntu/Debian + Apache

1. Запустите эту команду в консоли:

   ```
   sudo apt-get install php5-curl
   ```
       
2. Перезапустите Apache.
