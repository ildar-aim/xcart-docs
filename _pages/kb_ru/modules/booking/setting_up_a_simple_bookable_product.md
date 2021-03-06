---
lang: ru
layout: article_with_sidebar
updated_at: '2018-06-21 08:20 +0400'
identifier: ref_4lUFoqU2
title: Настройка простого бронируемого товара
order: 400
published: true
---
Создание бронируемого товара без вариантов:

-  {% link "Добавьте" ref_REno3u9g %} новый товар по обычным правилам. 
    ![1.jpg]({{site.baseurl}}/attachments/ref_4lUFoqU2/1.jpg)
    
-  В поле цена укажите стоимость бронирования объекта за одну ночь. 

Если цена будет изменяться, в этом поле будет указана базовая цена, а изменения цены будут отражены в опциях. Настройте {% link "опции товара с модификаторами цены" ref_SuWz9rmN %}. 

  В поле **Остаток** укажите максимально возможное количество единовременных бронирований. 
    
  **Пример:** В наличии 8 велосипедов, поэтому независимо от даты должно быть оформлено не более 8 прокатов велосипеда. В поле **Остаток товара Велосипед** следует указать 8.
  
  Резервируемые объекты не требуют доставки, и нет необходимости рассчитывать стоимость доставки. Установите значение **НЕТ** для опции **Требуется доставка**.
    
-  Заполните оставшиеся поля и сохраните новый товар.

-  Сохраните новый товар и перейдите на вкладку **Бронирование**:
    ![4.jpg]({{site.baseurl}}/attachments/ref_4lUFoqU2/4.jpg)
    
    **Бронирование** - Установите значение **Включено**, чтобы сделать объект доступным для бронирования.
    
    **Минимальный срок бронирования (количество ночей)** - Минимальный период времени, на который можно забронировать объект. Исчисляется в количестве ночей.
    
-  Будет полезно предоставить покупателям дополнительную информацию об объекте или о дополнительных опциях. Дополнительную информацию содержат {% link "атрибуты" ref_d0BOqdWu %}, настройте их для товаров. 
    Например, настройте дополнительные услуги за отдельную плату:
    ![5.jpg]({{site.baseurl}}/attachments/ref_4lUFoqU2/5.jpg)

Покупатели увидят новый объект для бронирования в магазине:

![]({{site.baseurl}}/attachments/8749984/8718726.png)

Нажав на название товара в форме бронирования, покупатель увидит детали предложения:

![]({{site.baseurl}}/attachments/8749984/8718727.png)

Стандартный текст модуля не подходит для всех видов бронируемых услуг и объектов. Например, для бронирования отелей и проката автомобилей требуют различных формулировок. Текст легко изменить в {% link "языковых переменных модуля" ref_5ic1ftH6 %}.
