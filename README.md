Android Studio Kotlin Каркас - макет. Иллюстрация компании разработки Подключение по API. https://stepik.org/lesson/780711/step/1?unit=783285
![10](https://user-images.githubusercontent.com/112688317/202256383-52b1f45c-a894-4dff-8437-dfd29f37d1a7.png)
<?версия xml="1.0" кодировка="utf-8"?>
<Линейное  описание xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity"
    android:orientation="vertical">

 
<!-- расположение на экране layout_gravity-->
<!-- start - влево, end - вправо-->
<!-- горизонтальная - bottom - вниз, top - вверх-->
<!-- match_parent - растягивает по ширине-->
 <Кнопка
         android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="button1"
        android:layout_weight="1"></Button>
    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="button2"
        android:layout_weight="2"
        android:layout_gravity="bottom"></Button>
    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="button3"
        android:layout_weight="2"
        android:layout_gravity="center_vertical"></Button>
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent " />

</LinearLayout>
![1111](https://user-images.githubusercontent.com/112688317/202257947-99979ad3-6cf5-45cb-8fe8-f896d92c9f5b.png)
<?версия xml="1.0" кодировка="utf-8"?>
<Линейное  описание xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity"
    android:orientation="vertical"
    android:gravity="center">

 <TextView
         android:id="@+id/TextView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android: layout_gravity="center"
        android:text="Привет, мир!"
        android:textSize ="50sp"
 />
 <Просмотр
         изображения android:layout_width="wrap_content"
        android:layout_height="302dp"
        android: src="@drawable/name">

 </ImageView>
 <Линейное
         описание android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_gravity="center"
 >


 <Кнопка
             android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="center"
            android:text="Button2"
 />

 <Кнопка
             android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="center"
            android:text="Button3"
 />

        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="center"
            android:text="Button1"
 />

    </LinearLayout>
</LinearLayout>
![qqqqqqq](https://user-images.githubusercontent.com/112688317/202258025-ab7d3782-12fc-42cc-87a2-dfcdc61c815d.png)
<?xml version="1.0" encoding="utf-8"?>
<FrameLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity"
    android:orientation="vertical"
    android:gravity="center">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:textSize="50sp"
        android:text="Dead!"
        android:layout_gravity="center"/>

    <ImageView
        android:layout_width="wrap_content"
        android:layout_height="302dp"
        android:src="@drawable/Лого">

    </ImageView>

        <Button
            android:layout_width="wrap_content"
            android:layout_height="265dp"
            android:layout_weight="8"
            android:text="Button1"
            android:layout_marginRight="50dp"
            android:layout_gravity="end|bottom"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="113dp"
            android:layout_weight="1"
            android:text="Button2"
            android:layout_marginLeft="50dp"
            android:layout_gravity="start|bottom"/>
        <Button
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="2"
            android:layout_marginTop="50dp"
            android:text="Button3"
            android:layout_gravity="center"/>


</FrameLayout>

Технологии разработки мобильный приложений Выделяют: destkop(настольные), мобильные, веб(сайты) Есть платформы: Android, IOS Способы разработки: Нативный, Гибридный, Кроссплатформенный

Нативный подход: Native - естественный для данной среды

Использование оригинальных языков Отдельное приложение для каждой платформы Сложные приложения требующие много ресурсов Гибридный подход:

Использование технологий веб-раззработки: JavaScript, CSS Приложения хорошо подходят для просмотра интернет-контента Созданный код работает внутри нативного приложения(Оболочки) Кроссплатформенный подход:

Полезны там, где не нужно применять сложный код Возможность работы на обеих платформах Приложение работают медленне по сравнению с нативными Насколько важны интерактивные элементы интерфейса? На каких платформах/типах устройство должно работать приложение? Необходим ли доступ к дополнительным функция и датчикам устройства? Какой бюджет и какие сроки разработки? История версий Android Создатель Android - Энди Рубин 5 ноября 2005 - день рождение Android

Android -студия Проблемы: Путь не должен содержать русских букв

Основы структуры мобильных приложений Язык программирвоания - Kotlin SDK - software development kit - Android Studio APK - формат архивных исполняемых файлов-приложений для Android

Каждое приложение Android работает в собственной песочнице (изолированной программной среде) за счёт вертуальной машины ОС Android = многопользовательский Linux У каждого приложения уникальный идентификатор который устанавливает полномочия

Предоставление ресурсов За счёт общего идентификатора(использования вертуальной машины)

Компаненты приложений Activity - дизайн Service - фоновые процессы Content Provider - база данных Broadcast receiver - уведомления(низкий заряд)

Ресурсы приложений изображение У каждого ресурса уникальный идентификатор

Структура проекта в Android Studio Отображение: Project(расположение на диске) и Android(по типам файлов) Android: App - программый код, ресурсы Gradle scripts - подключение сторонних библиотек Res - ресурсы, папки от плотнисти пикселей Drawable - фигуры и цвет Layout - внешний вид окон приложения Mipmap - значки приложения Values - ресурсы цветов, стили изображение manifests - предоставление основной информации о программе(какой java пакет, строки с 7 по 9 иконка прилежения, название в верхней строке, круглая иконка) изображение build.gradle - Версия SDK, => dependencies: зависимости - внешние библеотеки(доступ к сети) изображение

Код - внешний вид Наше приложенеие находится в папке layout в activity_main

Классы Класс хранится в папке java, также в папке приложения

Activity и макеты Макет - определяет способ представления интерфейса Activity - определяет действия

Алгоритм работы Устройство запускает приложение и создаёт Activity Activity задаёт макет Avtivity приказывает Android вывести макет на экран изображение Пользаватель взаимодействует с макетом Activity реагирует на взаимодействия, выполняя код прилодения Activity обновляет содержимое экрана Пользователь видит это на устройстве изображение Activity_main.xml - Код, Разделение, Дизайн

Структура Элементы типа View: кнопка, надпись, переключатель TextView Элементы типа GroupView: панельки, вкладки, контейнер ConstraintLayout Интерфейс - xml Макет LinearLayout Линейный макет, элемент идут друг за другом, слева направо

Макет FrameLayout Особенность Frame:позволяет использовать |

Макет ConstraintLayout gravity/margin не работает расположение вручную не отображается при запуске отсутствие ограничений - подчёркивает красным

Android — свободная операционная система для мобильных телефонов, планшетных компьютеров, умных часов, телевизоров и смартбуков, использующая ядро Linux, разрабатываемая Open Handset Alliance и принадлежащая Google. С момента выхода первой версии в сентябре 2008 года произошло 40 обновлений системы. Эти обновления, как правило, касаются исправления обнаруженных ошибок и добавления новой функциональности в систему.

Изначально Google рассчитывала давать версиям Android имена известных роботов, но отказалась из-за проблем с авторскими правами. Каждая версия системы, начиная с версии 1.5, получает собственное кодовое имя на тему сладостей. Кодовые имена присваиваются в алфавитном порядке латинского алфавита. Начиная с версии Android 10 кодовое название ОС получает только во время разработки. Начиная с версии 3.1 обновления будут выходить раз в 6 месяцев.

Также была версия Android 3.0 с кодовым названием Honeycomb, которая была нацелена на использование в устройствах с большим экраном, например планшеты. Данная версия довольно быстро перестала быть актуальной ввиду отсутствия в то время устройств с большим экраном, потому в 2012 году её поддержка закончилась.[1]

Последняя версия ОС Android на данный момент — Android 13, выпущенная 15 августа 2022 года.

Минимальная поддержка — Android KitKat.

Официальное приложение YouTube поддерживается на Android Lollipop и выше.

Сервисы Google Play поддерживаются приблизительно 10 лет с момента выхода Android.

Самая популярная версия — Android 11 (Red Velvet Cake) (27%). 27 сентября 2021 года Google закрыл доступ к аккаунтам пользователей на устаревших версиях ниже Android Honeycomb.[2]
