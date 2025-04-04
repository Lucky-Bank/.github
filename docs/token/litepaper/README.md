---
description: Lucky Bank — Кредитование под залог NFT
icon: rocket-launch
---

# Litepaper

## **1. Введение**

**Lucky Bank** — это инновационная платформа для кредитования под залог NFT, которая предлагает **качественный сервис**, **гибкие условия** и **уникальные возможности** для владельцев NFT и инвесторов. Сервис был запущен 6 декабря 2024 года, и на данный момент в нём реализован следующий функционал:

#### 1. Pool-to-peer NFT lending

Автоматические бессрочные займы в TON с гибкими настройками суммы и срока возврата кредита.

#### 2. Liquidity vault

Пассивный доход для инвесторов, разместивших свои средства в пуле автоматического кредитования.

#### 3. USDT lending

Мы первые в сети TON реализовали систему смарт-контрактов, позволяющую производить pool-to-peer кредитование в USDT под залог NFT (вместе с USDT пулом ликвидности соответственно).

#### 4. Аукционы

Залоговые NFT из просроченных кредитов автоматически поступают на аукцион.

***

## **2. Проблема**

> _Монополии очень вредны для развития экономики хотя бы потому, что они устанавливают высокие цены за далеко не всегда качественную продукцию. И конечно, в итоге "каннибализируют" сами себя, свои же технологии._\
> Жан Тироль
>
> _Всякая монополия... порождает неизбежно стремление к застою и загниванию_\
> В. И. Ленин

Исторически сложилось, что кредитование под залог NFT в сети TON монополизировано. С появлением на рынке кредитования Krediton Lending Tool (подробнее в разделе [Аналитика рынка](market-analysis.md)) рынок не смог ответить ничем, кроме демпинга ставок кредитования. Единственный игрок диктует высокие комиссии и негибкие условия, к тому же отсутствует информация о рисках[ (закрытые смарт-контракты)](#user-content-fn-1)[^1].

В сложившейся ситуации не происходит появление новых DeFi-инструментов, связанных с кредитованием под залог NFT, что, в свою очередь, тормозит развитие экосистемы TON в целом.

***

## **3. Решение**

Оценив объём рынка pool-to-peer кредитования под залог NFT, мы решили не входить в прямую конкуренцию с существующими участниками, так как это неизбежно повлечёт за собой "демпинговые войны" и в итоге не пойдёт на пользу никому. Поэтому в рамках дальнейшего развития Lucky Bank мы собираемся занять свободные ниши, а также попытаться создать новые инструменты DeFi, использующие NFT. Планируется в ближайшее время реализовать следующий основной функционал:

#### 1. AMM Telegram Gifts lending

В связи с появлением коллекций Telegram Gifts, у которых присутствует активный рынок и достаточно огромный саплай NFT, появляется возможность создания AMM пулов кредитования:

* Заёмщик токенизирует свой флорный подарок, путём отправки NFT на специальный контракт, который в обмен вернёт 1 токен, соответствующий этой коллекции подарков.
* Заёмщик обменивает полученный токен в AMM пуле на TON (или USDT) по текущему курсу обмена.
* Когда заёмщику будет необходимо вернуть кредит, он производит обратные действия: обменивает TON на токен необходимой коллекции и "выкупает" со смарт-контракта свой подарок или любой другой свободный для выкупа.
* Смарт-контракт ограничивает доступное время обмена токена заёмщика именно на его NFT, таким образом достигается некоторая "обезличенность" подарков, и основным параметром становится только их флор.
* В интерфейсе dApp все перечисленные процессы могут быть не видны. Заёмщик просто отправляет NFT, в ответ получает TON, и наоборот при возврате кредита в срок.
* Для инвесторов AMM пул кредитования практически ничем не отличается от стандартных пулов ликвидности DEX, кроме того, что у этих пулов значительно выше комиссии на обмены, а для того чтобы пополнить ликвидность, необходимо в паре с TON/USDT вносить ещё и NFT соответствующих коллекций.
* При достаточной востребованности данного вида кредитования появится возможность вынести его в отдельный сервис, и тем самым в экосистеме TON может появиться новый протокол — AMM NFT Marketplace.

#### 2. Peer-to-peer NFT lending

Такая технология уже успешно существовала в сети TON, но на данный момент эта ниша освободилась. Займы будут реализованы в TON и USDT. Процесс состоит из следующих этапов:

* Заёмщик присылает NFT на оценку банкирам.
* Банкиры присылают заёмщику свои предложения по сумме, сроку и процентной ставке кредита.
* Заёмщик выбирает лучшее предложение и получает кредит.

#### 3. Automated Peer-to-peer NFT lending

За счёт накопленного опыта в разработке смарт-контрактов pool-to-peer у нас есть возможность расширить стандартное peer-to-peer кредитование и тем самым упростить/ускорить получение кредита заёмщиком:

* Банкир создаёт свой собственный пул ликвидности и настраивает параметры кредитования интересующих его коллекций.
* Заёмщик выбирает лучшее предложение из заранее созданных и получает кредит.

Более подробно с планом развития и разработки можно ознакомиться в разделе [Дорожная карта](roadmap.md).

***

## **4. Финансовая модель**

* **Источники дохода**:
  * Комиссия за выдачу кредита (конкурентоспособные ставки, без демпинга).
  * Процентная ставка по кредиту (рыночные условия).
  * Штрафы за просрочку платежей.
  * Комиссия за P2P-кредитование.
  * Комиссия за AMM-кредитование.
* **Расходы**:
  * Разработка и поддержка платформы.
  * Маркетинг и привлечение пользователей.
  * Резервы на пополнение пула автоматического кредитования.
  * Резервы на пополнение пула AMM кредитования.
*   **Цели**:\
    Выйти за год на доходность проекта в месяц:

    * Пессимистичный сценарий: 3750 USDT
    * Оптимистичный сценарий: 14000 USDT

    Более подробно в разделе [Аналитика рынка](market-analysis.md)

***

## **5. Токеномика**

В целях реализации намеченных планов дальнейшего развития Lucky Bank потребуется привлечение дополнительных инвестиций. Привлечение инвестиций планируется произвести с помощью реализации токена проекта.

Тикер: _**$BANK**_\
Общее количество токенов: **100 000**\
Адрес мастер-контракта: [**EQB1399hPqWDdupmVw43dKBEgYgsEtoliVGsfpchiHC-BANK**](https://tonviewer.com/EQB1399hPqWDdupmVw43dKBEgYgsEtoliVGsfpchiHC-BANK)\
Owner: _**Отозван**_\
Формат ICO: _**Public Sale. Квадратичная кривая. Старт 1 USDT. Окончание 3 USDT.**_\
Soft Cap: _**5000 (12.04.2025)**_

Подробнее в разделе [Токеномика](tokenomiks.md).

***

## **6. Преимущества для холдеров токена**

* **Стейкинг.** Часть комиссий сервиса будет распределяться между холдерами токена путём его стейкинга.
* **Увеличенный пассивный доход.** Холдерам токена будет предоставлен доступ к пулам кредитования с более высоким utilization rate (тем самым и с более высоким APY).
* **Доступ к p2p.** Кредитование поступивших заявок будет доступно только холдерам токена. Также от количества токенов будет зависеть размер взимаемой комиссии сервиса.
* **Доступ в приватный чат банкиров.** Приватный чат доступ в который имеют люди, заинтересованные в выдаче кредитов под ликвидные/красивые нфт, которые им тоже интересны. Общение, советы и инсайды.

***

## **9. Команда**

* **CEO**/**CTO**: Павел.\
  Telegram: [@x1y1x3](https://t.me/x1y1x3)\
  Фуллстэк программист (общий опыт в программировании начиная с 1994 года).\
  Основная специализация/работа — f2p-игры для социальных сетей (с 2009 года).\
  Опыт программирования смарт-контрактов в сети TON (с 2023 года).\
  Реализовано: Система смарт-контрактов кредитования под залог NFT для TON Lombard bot, контракт-контейнер Lucky Wallet (полуфиналист TON Open League Hackathon 2024) и Krediton Lending Tool (также попал в топ-100 проектов хакатона).
* **CM**: Soon.

***

## **10. Заключение**

**Lucky Bank** предлагает **альтернативу монополисту**, предоставляя пользователям **качественный сервис**, **прозрачность** и **уникальные возможности**. Мы стремимся стать **лидером рынка**, используя инновационные технологии и предоставляя пользователям больше свободы и выбора. Токен $BANK будет играть ключевую роль в экосистеме, обеспечивая утилиты и стимулы для участников.

## **Ссылки**

$BANK Public Sale: [https://lucky-bank.github.io/public-sale/](https://lucky-bank.github.io/public-sale/)

Telegram MiniApp: [https://t.me/Lucky\_BankBot/App](https://t.me/Lucky_BankBot/App)\
Web: [https://lucky-bank.github.io/](https://lucky-bank.github.io/)

Telegram Channel (RU): [https://t.me/lucky\_ton\_bank](https://t.me/lucky_ton_bank)\
Telegram Chat: [https://t.me/lucky\_bank\_chat](https://t.me/lucky_bank_chat)

[^1]: Смарт-контракт кредита KLT верифицирован, объявлено Bugbounty https://t.me/krediton\_official/18
