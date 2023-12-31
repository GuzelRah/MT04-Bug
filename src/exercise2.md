﻿# Баг-репорты

## Баг №1. Логин в поле "Username" всегда вводится с заглавной буквы.

Предшествующие условия:\
Пользователь находится на странице авторизации.

Серьёзность:\
Blocker

Шаги для воспроизведения:
1. Ввести логин "admin" в поле "Username".

Ожидаемый результат:\
В поле "Username" написано "admin".

Фактический результат:\
Поле "Username" всегда вводится с заглавной буквы ("Аdmin"), невозможно зайти в приложение.

## Баг №2. В форме авторизации не выводится нужное сообщение при пустом поле.

Предшествующие условия:\
Пользователь находится на странице авторизации.

Серьёзность:\
Trivial

Шаги для воспроизведения:

1. Поле "Username" оставить пустым;
1. В поле "Password" ввести "admin";
1. Нажать кнопку "Log in".

Ожидаемый результат:\
В форме авторизации выводится сообщение "Enter Both Username And Password".

Фактический результат:\
В форме авторизации выводится сообщение "Please Enter Bouth Username And Password".

## Баг №3. В форме авторизации не выводится нужное сообщение при неверном логине.

Предшествующие условия:\
Пользователь находится на странице авторизации.

Серьёзность:\
Trivial

Шаги для воспроизведения:

1. Поле "Username" ввести неверный логин;
1. В поле "Password" ввести "admin";
1. Нажать кнопку "Log in".

Ожидаемый результат:\
В форме авторизации выводится сообщение "Username Not Found".

Фактический результат:\
В форме авторизации выводится сообщение "Username Not FoundLog In Successfull".

## Баг №4. Сообщение о неверном логине выводится в левом верхнем углу экрана.

Предшествующие условия:\
Пользователь находится на странице авторизации.

Серьёзность:\
Trivial

Шаги для воспроизведения:

1. Поле "Username" ввести неверный логин;
1. В поле "Password" ввести "admin"";
1. Нажать кнопку "Log in".

Ожидаемый результат:\
Сообщение о неверном логине выводится над кнопкой "Log In".

Фактический результат:\
Сообщение о неверном логине выводится в левом верхнем углу экрана.

## Баг №5. Сообщение о пустом логине выводится в левом верхнем углу экрана.

Предшествующие условия:\
Пользователь находится на странице авторизации.

Серьёзность:\
Trivial

Шаги для воспроизведения:

1. Поле "Username" оставить пустым;
1. В поле "Password" ввести "admin"";
1. Нажать кнопку "Log in".

Ожидаемый результат:\
Сообщение о пустом логине выводится над кнопкой "Log In".

Фактический результат:\
Сообщение о пустом логине выводится в левом верхнем углу экрана.

## Баг №6. Выбранный язык сбрасывается после попытки авторизации.

Предшествующие условия:\
Пользователь находится на странице авторизации.

Серьёзность:\
Major

Шаги для воспроизведения:

1. В окне авторизации выбрать французский, итальянский или немецкий языки;
1. Поле "Username" оставить пустым;
1. В поле "Password" ввести "admin"";
1. Нажать кнопку "Log in".

Ожидаемый результат:\
После попытки авторизации выбранный язык не сбрасывается.

Фактический результат:\
После попытки авторизации интерфейс переключается на английский язык.
