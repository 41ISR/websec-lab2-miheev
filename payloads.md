# Payloads для gruyere

_Пример оформления работы_

## Payload 1

При регистрации находишь поле ввода названия профиля и в коде и меняшь параметр `value maxlength="16"` на например `"121"`. В название профиля пишешь `<script>alert('aye')</script>`. После регистрации заходим в `Sign in`. 

## Payload 2

Переходим в профиль и в поле `Profile color` пишем ` purple' onmouseover='alert("purple") ` и при навeдении на Ваше имя будет вызываться xss (поменять профиль колор уже не получится). 

## Payload 3

Загружаем файл любой.html с алертом и переходя по ссылке после загрузки.

## Payload 4

После авторизации добавляем новый пост с `<a onmouseover="alert('asd')" >asd</a>` и добавляем, будет вылазить уже сразу после публикации (в моих постах) и в `Home` тоже(хз считается это за 2 способа вызвать xss или 1)

## Payload 5

После авторизации можно просто написать алерт в строке поиска. Пример: `https://google-gruyere.appspot.com/564979828150736262886706255503895022888/asdasd/<script>alert('feq')</script>`
