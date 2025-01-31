# Film russian distribution data analysis/ Исследование данных о российском кинопрокате

## Цель проекта:
* изучить рынок российского кинопроката и выявить текущие тренды,
* изучить фильмы, которые получили государственную поддержку. Насколько такие фильмы интересны зрителю.
* изучить динамику выхода фильмов по годам
* изучить динамику сборов от проката фильмов по годам
* определить влияние возрастного ограничения насборы фильмов.

## Стек:
* pandas
* datetime
* matplotlib
* маркетинг-аналитик, аналитик (универсал), data analyst


# Выводы (статус проекта - завершен):
**Динамика проката фильмов по годам**
* Если смотреть просто по количеству фильмов за каждый год, то нет какой-либо зависимости, количество фильмов то растет, то снижается, только за последние 2 года (18-й и 19-й) количество фильмов в прокате увеличилось
* если смотреть на долю фильмов с информацией по сборам, то видно, что до 2013 года включительно такая доля < 30%
* в 2014 году доля таких фильмов уже 35%, а в 2015-2019гг доля таких фильмов в среднем 63%
   - это объясняется тем, что в 2014 году Фонд кино по заключенному государственному контракту от 12.05.2014г. №1252-01-41/03/14 стал опертором ЕАИС. Назначение указанной системы состоит в сборе, учёте и обработке сведений о публичной демонстрации кинофильмов в кинозалах российских кинотеатров. То есть до 2014 года, такие данные централизованно не обрабатывались: https://ekinobilet.fond-kino.ru/about/history/

**Динамика сборов по годам**
* с 2010 по 2013 количество сборов примерно на одном уровне ~ 13,32 млн.р
* резкий скачок в 2014 году до 7.44 млрд.р в связи с контрактом от 12.05.2014г. №1252-01-41/03/14
* с 2014 года медианные значения на порядок меньше средних - это говорит о том, что каждый год есть несколько кассовых фильмов, сборы которых очень высокие по сравнению с остальными фильмами.


**Зависимость рейтинга от возрастного ограничения**
* От года к году картина немного меняется:
  - в 2019 год, почти одинаковое распределение между категориями "6+", "16+", "12+", лишь немного вперед ушла категория "6+"
  - категории "6+" и "12+" постоянно меняются местами
В целом наблюдается тенденция снижения возрастного ограничения, то есть все больше фильмов подходят для семейного просмотра, таким образом, увеличивают охват аудитории
  

**Зависят ли сборы и рейтинг от жанра**

* рейтинг не зависит от жанра, все-таки это очень индивидуально, по данным жанр "аниме" самый крутой, но количество фильмов в этом жане не очень большое, видимо, зрители аниме более лояльного склада характера при оценке, чем, например зрители ужасов. В ужасах наоборот довольно большое количество фильмов с данными, но если зритель — "эксперт" по ужасам, то он будет ставить низкий рейтинг даже на страшные фильмы по мнению большинства, а если фильм прям жуть жуткий, то он тоже может получить низкий рейтинг от этого самого большинства или вообще не быть просмотренным
* а вот сборы зависят от жанра
* самый кассовый жанр — спорт (если взглянуть на список фильмов, то кассовость жанра определил фильм "Движение вверх" (2017))
* остальные жанры практически ожидаемо заняли свои места, напишу первые 3 после спорта:
  - 2-е место: фантастика (это все супергеройские фильмы)
  - 3: фэнтези
  - 4: боевик
* на фильмы этих жанров идут с большей вероятностью, чем на другие 

