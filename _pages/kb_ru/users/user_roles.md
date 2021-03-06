---
lang: ru
layout: article_with_sidebar
updated_at: '2018-01-05 14:38 +0400'
title: Роли пользователей магазина
order: 20
published: true
identifier: ref_roles
---
Если в магазине несколько администраторов, роли определяют для них разный уровень доступа в панель управления магазина. Роль - это набор прав, дающих доступ к тем или иным функциям и разделам в интерфейсе администратора. Роли помогают распределять обязанности между сотрудниками или группами сотрудников магазина.

Настройка ролей возможна после установки и активации модуля **User Permissions**, который входит в пакеты X-Cart Business, Multivendor и Ultimate.
    ![1.jpg]({{site.baseurl}}/attachments/ref_roles/1.jpg)

В магазинах на базе X-Cart Business, Multivendor и Ultimate модуль активирован по умолчанию, и настроено несколько ролей. Список ролей доступен на странице **Пользователи / Роли**.
    ![2.jpg]({{site.baseurl}}/attachments/ref_roles/2.jpg)

Роль _Администратор_ имеет полный неограниченный доступ в панель управления магазина.

Остальные роли предоставляют ограниченный доступ к определенным разделам посредством прав:

    * Управление каталогом - право работать с запасом товаров;
    * Управление пользователями - право редактировать учетные записи пользователей;
    * Управление заказами - право просматривать и изменять заказы.

Список прав увеличивается с установкой модулей. Например, модуль **Simple CMS** добавляет два права:

    * Управление созданными страницами - право редактировать созданные дополнительные страницы;
    * Управление меню - право редактировать главное меню и меню в нижней части страницы.

Чтобы узнать, какими правами обладает та или иная роль, нажмите на ее название. Например, проверим _Управление купонами_:
    ![3.jpg]({{site.baseurl}}/attachments/ref_roles/3.jpg)

У роли _Управление купонами_ только одно право - управление купонами. Это значит, что администратор видит только раздел редактирования купонов и меню в панели управления магазина:
    ![4.jpg]({{site.baseurl}}/attachments/ref_roles/4.jpg)

Администратор может работать со страницей  **Скидки / Купоны** (создавать, просматривать, редактировать и удалять купоны).
    ![5.jpg]({{site.baseurl}}/attachments/ref_roles/5.jpg)

Роли можно удалять, настраивать в соответствии с требованиями работы магазина и создавать новые.

Как создать новую роль:
1.  Нажмите **Новая роль**.
    ![6.jpg]({{site.baseurl}}/attachments/ref_roles/6.jpg)

2.  На открывшейся странице укажите данные новой роли:
    ![7.jpg]({{site.baseurl}}/attachments/ref_roles/7.jpg)

     *   Название: Название роли.
     *   Включено: включение и отключение роли. Если роль отключена, пользователи с этой ролью могут войти в интерфейс администратора, но не видят разделов, в которым дает доступ их роль.
     *   Права: набор возможностей для пользователя с этой ролью. Начните печатать, появится список прав, соответствующих введенному ключевому слову, из которого вы можете выбрать нужные.

3.  Нажмите **Создать**.

Для редактирования роли нажмите на ее название в списке, измените данные и нажмите **Обновить**. 

Для удаления роли нажмите на значок корзины справа от названия и нажмите **Сохранить**.

Чтобы отключить роль и права, которые она дает, нажмите на зеленый переключатель слева от названия и нажмите **Сохранить**:
    ![8.jpg]({{site.baseurl}}/attachments/ref_roles/8.jpg)
    
Чтобы присвоить роль пользователю, измените профиль пользователя:
    ![9.jpg]({{site.baseurl}}/attachments/ref_roles/9.jpg)

Один пользователь может обладать несколькими ролями .
