#### *Библиотека основана на ресурсах сообщества и поддерживается основателями проектов [21 идея](https://www.21ideas.org/) и [Биткоин абстракцион](https://t.me/bitraction).* 

> Подписывайся на нас в любимом Nostr-клиенте:
>> @Tony - `npub10awzknjg5r5lajnr53438ndcyjylgqsrnrtq5grs495v42qc6awsj45ys7`
>> 
>> @almoo - `npub1zvvv8fm7w2ngwdyszg3y6zgp6vwqlht8zrr8wcmjaxjecrvpjfwsd0zs7w`

## Оглавление:
1. [Что такое Nostr?](https://nostr.21ideas.org#-%D1%87%D1%82%D0%BE-%D1%82%D0%B0%D0%BA%D0%BE%D0%B5-nostr)
2. [Ключи](https://nostr.21ideas.org#%EF%B8%8F-%D0%BA%D0%BB%D1%8E%D1%87%D0%B8)
3. [Клиенты](https://nostr.21ideas.org#-%D0%BA%D0%BB%D0%B8%D0%B5%D0%BD%D1%82%D1%8B)
6. [Обозреватели релеев](https://nostr.21ideas.org#-%D0%BE%D0%B1%D0%BE%D0%B7%D1%80%D0%B5%D0%B2%D0%B0%D1%82%D0%B5%D0%BB%D0%B8-%D1%80%D0%B5%D0%BB%D0%B5%D0%B5%D0%B2)
7. [Дополнительные ресурсы](https://nostr.21ideas.org#-%D1%80%D0%B5%D1%81%D1%83%D1%80%D1%81%D1%8B)
8. [Биткоин-онли ресурсы](https://nostr.21ideas.org#-%D0%B1%D0%B8%D1%82%D0%BA%D0%BE%D0%B8%D0%BD-%D0%BE%D0%BD%D0%BB%D0%B8-%D1%80%D0%B5%D1%81%D1%83%D1%80%D1%81%D1%8B)

![Nostriches everywhere](https://raw.githubusercontent.com/bitcoin21ideas/nostr/main/images/photo_2023-02-02%2011.14.55.jpeg)
*Изображение украдено у Егора Петрова (публичный ключ: `npub1z4m7gkva6yxgvdyclc7zp0vz4ta0s2d9jh8g83w03tp5vdf3kzdsxana6p`)*

***

# 🧐 Что такое Nostr?
Nostr – новый и непривычный, но в то же время очень крутой протокол. Это простейший открытый протокол, способный раз и навсегда создать устойчивую к цензуре глобальную "социальную" сеть.

* Он не зависит от какого-либо доверенного центрального сервера, поэтому он устойчив к цензуре.
* Он основан на криптографических ключах и подписях, поэтому он устойчив к взлому.

*Конструкция nostr очень проста*
* Есть два компонента: клиенты и релеи (ретрансляторы). Каждый пользователь запускает клиент. Любой пользователь может управлять ретранслятором.
* Каждый пользователь идентифицируется с помощью открытого ключа. Каждое сообщение подписывается. Каждый клиент проверяет эти подписи.
* Клиенты получают данные от выбранных ими релеев и публикуют данные другим релеям на свой выбор. Релеи не общается с другими релеями, только напрямую с пользователями.

*Чтобы использовать nostr, вам потребуется [ключ](https://nostr.21ideas.org#%EF%B8%8F-%D0%BA%D0%BB%D1%8E%D1%87%D0%B8) и [клиент](https://nostr.21ideas.org#-%D0%BA%D0%BB%D0%B8%D0%B5%D0%BD%D1%82%D1%8B)*
* Каждый использует свой клиент. Это может быть нативный клиент, веб-клиент и т.д.
* Чтобы опубликовать что-то, вы пишете сообщение, подписываете его своим ключом и отправляете на несколько релеев (серверов, размещенных кем-то другим или вами).
* Чтобы получить обновления от других людей, вы спрашиваете у нескольких релеев, знают ли они что-нибудь об активности этих пользователей в сети.
* Любой желающий может управлять релеем. Релей очень прост и даже глуп. Он не делает ничего, кроме как принимает сообщения от одних пользователей и пересылает их другим.
* Релеи не требуют доверия. Подписи проверяются на стороне клиента.

***

# 🗝️ Ключи
Ваши ключи – это ваша личность. Вы можете считать свой открытый ключ (`npub...`) своим именем пользователя, а свой закрытый ключ (`nsec...`) – своим паролем.

### ⚠️ Не вставляйте свой закрытый ключ в поля на веб-сайтах ⚠️

### 🔒 Храните ключи в безопасном месте и не делитесь своим закрытым ключом 🔒

Ключи существуют в двух форматах – шестнадцатеричном `hex` и вышеупомянутом `npub`/`nsec`. Для преобразования между этими двумя форматами можно использовать [инструмент конвертации ключей](damus.io/key).

***

# 🔐 Менеджмент ключей Nostr
Расширения ниже помогут вам сгенерировать свою пару ключей, а так же устранят необходимость раскрытия приватного ключа при входе в веб-клиенты Nostr. Используйте их для менеджмента и общего повышения безопасности ваших ключей.

* [Nos2x](https://github.com/fiatjaf/nos2x) — расширение от `@fiatjaf`, создателя протокола Nostr
* [Alby](https://getalby.com/) — расширение для браузерных Lightning платежей с встроенной поддержкой Nostr

Расширения работают локально, так что генерируйте свой ключ, отключив интернет, и сохраняйте физический бэкап вашей пары.

***

# 📱 Клиенты
Клиенты – это просто приложения, через которые вы можете взаимодействовать с протоколом Nostr. Подобно тому, как вы можете скачать разные приложения для взаимодействия с Telegram или Twitter. Периодически заглядывайте на [nostr.net#clients](https://nostr.net#clients), где хранится список клиентов, а также обратите внимание на [сравнительную таблицу клиентов](https://github.com/vishalxl/Nostr-Clients-Features-List#nostr-client-feature-list).

## Web
* [nostr.rocks](https://nostr.rocks/)
* [astral.ninja](https://astral.ninja/)
* [snort.social](https://snort.social/)
* [yosup.app](https://yosup.app/)

## Android
* [Amethyst](https://play.google.com/store/apps/details?id=com.vitorpamplona.amethyst&hl=en)
* [Daisy](https://neb.lol/nostr) (APK)

## iOS
* [Damus](https://damus.io/)
* [Daisy](https://neb.lol/nostr)

***

# 📥 Обозреватели релеев
Чтобы клиент работал, его нужно подключить к ретранслятору. Можно как запустить собственный ретранслятор, так и присоединиться к уже запущенным.

* [nostr.watch](nostr.watch/relays/find)
* [nostr.info](nostr.info/relays/)

***

# 🧮 Генераторы Vanity адресов
Генераторы Vanity адресов позволяют создать публичный ключ Nostr, который будет начинаться (или заканчиваться) на выбранные вами символы. Такая утилита позволяет добавить немного персонализации вашему адресу. Учтите, что чем больше символов вы хотите добавить, тем больше времени займет Proof-of-Work генерация такого адреса(зависит от мощности вашего компьютера)

> Например, поиск
> 
> 1 символа может занять до 0.1 секунды
> 
> 2 символов может занять до 1 секунды
> 
> 3 символов = может занять до 30 секунд
> 
> 4 символов = может занять до 10 минут
> 
> 5 символов = может занять до 1 часа
> 
> 6+ символов = несите огнетушитель и да поможет вам бог!

* [hitony.com](https://hitony.com/nostrogen/) — bech32 генератор (npub1)
* [nostr.rest](https://www.nostr.rest/) — генератор адресов через хеширование

***

# 📚 Ресурсы
Больше информации о протоколе Nostr можно узнать здесь:

* [nostr.net](https://www.nostr.net/) — список проектов Nostr
* [nostr-resources.com](https://nostr-resources.com/) — ресурс Gigi, послуживший основой для [nostr.21ideas.org](https://nostr.21ideas.org/)
* [uselessshit.co](https://uselessshit.co/resources/nostr/) — F.A.Q.
* [nostr.directory](https://nostr.directory/) — поиск людей из Twitter

***

# 💡 Биткоин-онли ресурсы
Не забывай, что Nostr активно поддерживает Биткоин, и в протокол уже внедрена сеть Молния. Поэтому обрати внимание на ресурсы ниже:

* Web: [21ideas.org](https://www.21ideas.org/)
* Telegram: [t.me/bitcoin21ideas](https://t.me/bitcoin21ideas)
* YouTube: [@21ideas](https://www.youtube.com/@21ideas/)

***

# 🍩 Поддержи проект
Материал оказался полезен? Купи нам пару баночек пива 🍻 через сеть Lightning⚡️

⚡️21ideas@getalby.con
![LNURL_QR](https://github.com/bitcoin21ideas/nostr/blob/main/images/LNURL%20QR.png?raw=true)
`LNURL1DP68GURN8GHJ7MR9VAJKUEPWD3HXY6T5WVHXXMMD9AKXUATJD3CZ7KN409PRX3SL5GSK5`

***

![purple_bitcoin](https://github.com/bitcoin21ideas/nostr/blob/4a7975167a0da202b8439f8b0f5addd915d7aab0/images/photo_2023-02-03%2014.50.43.jpeg?raw=true)
