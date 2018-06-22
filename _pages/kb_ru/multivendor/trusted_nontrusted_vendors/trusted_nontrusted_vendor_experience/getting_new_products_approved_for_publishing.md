---
lang: ru
layout: article_with_sidebar
updated_at: '2018-06-21 23:27 +0400'
identifier: ref_2fNSmNFO
title: Отправка нового товара на проверку (для продавцов со статусом Ненадёжный)
order: 460
published: true
---
Если в _X-Cart Мультивендор_ активирован модуль **Надёжные и ненадёжные продавцы (Trusted/Non-trusted vendors)**, администратор разделяет продавцов на проверенных и непроверенных. 

Новые товары продавцов со статусом **Надёжный** сразу появляются в каталоге магазина. 

Продавцы со статусом **Ненадёжный** отправляют новые товары на проверку администратору, и товары появляются в магазине, только если одобрены администратором. 

В панели управления продавца опция включения товара неактивна, пока товар находится на проверке у администратора. Товар активируется, если администратор его одобряет, и остаётся отключённым - если отклоняет.
![1.jpg]({{site.baseurl}}/attachments/ref_2fNSmNFO/1.jpg)

Ненадёжный продавец сохраняет новый товар и в нижней части страницы видит статус **Товар не одобрен**. Кнопка **Отправить на одобрение** передаёт товар администратору на проверку:
![2.jpg]({{site.baseurl}}/attachments/ref_2fNSmNFO/2.jpg)

Как только продавец отправляет товар на проверку, статус изменяется на **Товар отправлен на одобрение**:
![3.jpg]({{site.baseurl}}/attachments/ref_2fNSmNFO/3.jpg)

Далее продавец ожидает результатов проверки - администратор одобряет или отклоняет товар. Результат проверки и комментарии администратора отправляются продаву по электронной почте. Соответственно, статус товара изменяется на **Товар одобрен**:
![4.jpg]({{site.baseurl}}/attachments/ref_2fNSmNFO/4.jpg)

или **Товар отклонён**:
![5.jpg]({{site.baseurl}}/attachments/ref_2fNSmNFO/5.jpg)

Если товар не прошёл проверку, продавец корректирует информацию о товаре, как администратор советует в комментариях, и повторно передаёт товар на проверку. 

Кнопка **Отправить на одобрение** снова появляется на странице _отклонённого товара_, как только продавец обновляет товар. X-Cart не проверяет, какие изменения делает продавец, это не обязательно изменения, рекомендованные администратором.

_Одобренный товар_ сохраняет статус **Товар одобрен**, даже если продавец редактирует информацию о товаре.