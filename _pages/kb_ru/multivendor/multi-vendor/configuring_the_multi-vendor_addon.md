---
lang: ru
layout: article_with_sidebar
updated_at: '2018-06-18 23:01 +0400'
identifier: ref_3fL15c4m
title: Настройка модуля Multi-vendor
order: 150
published: true
---
В разделе **Мои модули** в панели управления магазина найдите модуль по названию **Multi-vendor** и пройдите по ссылке **Настройки**:
    
   ![2.jpg]({{site.baseurl}}/attachments/ref_3fL15c4m/2.jpg)

   *   **Режим работы Multivendor** - Что будет представлять из себя ваша торговая площадка - общий склад магазин, в котором разные продавцы предлагают свои товары, или отдельные склады каждого продавца.  

        <table class="ui compact celled small padded table">
      <thead>
        <tr class="sortableHeader">
          <th class="confluenceTh sortableHeader" data-column="0">
            <div class="tablesorter-header-inner">Общий склад</div>
          </th>
          <th class="confluenceTh sortableHeader" data-column="1">
            <div class="tablesorter-header-inner">Отдельные склады</div>
          </th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td class="confluenceTd">
            <ul>
              <li>Если покупатель выбирает товары разных продавцов, формируется один заказ.</li>
              <li>Администратор обрабатывает заказ. Продавец не имеют прав на редактирование заказа.</li>
              <li>Все товары заказа доставляются одной посылкой из единого магазина. Стоимость доставки рассчитывается с адреса компании, указанного администратором магазина в настройках .</li>
            </ul>
          </td>
          <td class="confluenceTd" >
            <ul>
              <li>Если покупатель выбирает товары разных продавцов, формируется отдельный заказ на товары каждого продавца.</li>
              <li>м.</li>
              <li>Каждый заказ отправляется из магазина продавца. Стоимость доставки рассчитывается с адреса, указанного продавцом.</li>
            </ul>
          </td>
        </tr>
      </tbody>
    </table>

### Финансы
    
   *   **Комиссия со стоимости товаров в заказе** и **Комиссия со стоимости доставки заказа** - Эти настройки устанавливают размер комиссии, которую продавец платит владельцу магазина с каждой продажи.
   
**Комиссия со стоимости товаров в заказе** - процент от стоимости товаров в заказе. **Комиссия со стоимости доставки заказа** - процент от стоимости доставки заказа. 

Эта настройка действует только в режиме **Отдельные склады**, т.к. в режиме **Общий склад** товары всех продавцов доставляются с одного склада и комиссия с доставки для каждого продавца не рассчитывается). Указанные в этих полях процентные ставки применяются ко всем продавцам, для которых не определены индивидуальные условия. Размер комиссии рассчитывается автоматически после оплаты покупателем заказа, содержащего товары продавца. 

Администратор видит размер полученной за каждый заказ комиссии в разделе **Заказы / Список заказов**. Администратор может установить индивидуальные условия расчёта для продавца, в этом случае размер комиссии задаётся в разделе Финансовые детали учётной записи продавца. 
        
   *   **За сбор и уплату налога с продаж отвечает** - Модуль **Multi-vendor** позволяет возложить обязанности по собру и уплате налогов на владельца торговой площадки или на каждого продавца в отдельности (настройка За сбор и уплату налога с продаж отвечает). 
   
   В магазинах, зарегистрированных на территории США, Великобритании и ЕС, администратор управляет налогами с помощью модулей **Sales tax, VAT/GST, Canadian taxes, AvaTax** и **TaxJar**, а продавцы - с помощью модулей **AvaTax** и **TaxJar**. 
   
   В магазинах, зарегистрированных на территории Российской Федерации, не применимы модули **VAT/GST** и **Canadian taxes**, т.к. не имеют отношения к российской системе налогообложения, и модули **AvaTax** и **TaxJar**, т.к. сервисы не действую на территории Российской Федерации. 
   
   Таким образом, функциональность магазина позволяет управлять налогами только администратору с помощью модуля **Sales tax**. Поэтому в российских магазинах значение настройки З**а сбор и уплату налога с продаж отвечает** всегда должно быть **Владелец сайта**. 
  
   *   **Минимальный баланс, при котором продавец может запросить выплату средств** - Минимальная сумма в рублях на счёте продавца, при которой продавец может запросить выплату выручки с продаж.
    
   *   **Высылать нотификацию при запросе на выплату средств** - Эта настройка включает и отключает уведомление по электронной почте **Запрос от продавца на выплату средств**. Это же уведомление администратор может настроить и редактировать в разделе **Настройка магазина / Уведомления по электронной почте**. Когда настройка включена, администратор получает email уведомление о запросе выплаты от продавца. Когда настройка отключена, администратор не получает уведомление, но видит запрос на выплату в списке платёжных операций в разделе **Заказы**.
    
   *   **Высылать запрос на выплату средств на e-mail** - Это поле отображается, только если включена настройка **Высылать нотификацию при запросе на выплату средств**. Уведомления о запросах на выплату будут высылаться на указанный адрес. Если оставить поле пустым, уведомления не будут высылаться.
    
   *   **Требовать загрузить инвойс при запросе на выплату средств** - Администратор может потребовать от продавца счёт на оплату для оформления выплаты. Если эта настройка включена, продавец не сможет запросить выплату без предоставления счёта. Счёт будет прикреплён к уведомлению по электронной почте **Запрос от продавца на выплату средств**, отправляемому на адрес, указанный в поле **Высылать запрос на выплату средств на e-mail**.
   
### Конфиденциальность и доступ к данным

   *   **Скрывать от продавца информацию о покупателе** - С помощью этой настройки администратор позволяет или не позволяет продавцам видеть контактную информацию покупателей.
    
   *   **Использование продавцом глобальных атрибутов** - Настройка определяет, разрешено или нет продавцам добавлять новые значения атрибутов (глобальных и в классах товаров), созданных админстратором и другими продавцами. Возможные варианты - **Может использовать только уже существующие значения** и **Может использовать существующие значения и создавать новые**.

   *   **Разрешить продавцам одобрять, отклонять и редактировать оценки и отзывы о товарах** - Настройка позволяет продавцам редактировать оценки и отзывы покупателей об их товарах.
   
   *   **Разрешить вендорам отвечать на оценки и отзывы о товарах** - Настройка позволяет продавцам отвечать на отзывы покупателей и комментировать оценки товаров.
   
### Внешний вид   

   *   **Тип оценки продавца** - Подробный отзыв или оценки товаров. 
   
   *   **Отображать список продавцов в фильтре товаров** - Настройка действует только при включённом модуле **Фильтры свойств товаров** (**Product Filter**). Если опция включена, в фильтрах для поиска товаров появится фильтр по названию магазина продавца, и покупатели смогу получить список товаров конкретного продавца. Поиск по продавцу работает только в категориях, содержащих товары нескольких продавцов.
   
   *   **Отображать список продавцов в боковой панели** - Если настройка включена, в боковой панели витрины магазина появится список продавцов, предлагающих свои товары на торговой площадке.
    
   *   **Отображать оценки продавца** - Эта настройка действует только при включённом модуле **Отзывы о товарах (Product Reviews)**.
    
### Начало работы   
    
   *   **Набор прав доступа, назначаемых новым продавцам по умолчанию** - Набор прав, доступный новому пользователю после создания учётной записи продавца администратором или после подтверждения администратором запроса на регистрацию в качестве продавца. После установки модуля **Multi-vendor** доступна только одна роль - **Продавец**. Администратор может создать дополнительные роли (наборы прав на управление) для пользователей, которые будут действовать в качестве продавцов. Настройка устанавливает набор прав для пользователей с уровнем доступа **Продавец**.
   
   *   **Ознакомительное сообщение для нового продавца** - Приветственное сообщение, которое увидят новые продавцы при первом входе в учётную запись в магазине.
   
   
