# Список ссылок докладу «[Тепловые карты на JavaScript](https://11.codefest.ru/lecture/1799)»

Презентация появятся на сайте [CodeFest](https://11.codefest.ru/lecture/1799) почти сразу после конференции, а запись должна появиться примерно в декабре 2021.

1. [Демо-стенд](https://kalyanov.github.io/idw/) с реализацией алгоритма IDW
1. [Репозиторий демо-стенда](https://github.com/kalyanov/idw)

## Познакомимся

1. [flamp.ru](https://flamp.ru) — сервис отзывов
1. [2gis.ru](https://2gis.ru) — онлайн-версия сервис 2ГИС
1. [Доклад «WebGL на карте. Карта на WebGL»](https://2019.codefest.ru/lecture/1426) про карту 2gis
1. [Публичный api](https://docs.2gis.com/ru/mapgl/overview) карты 2gis
1. [Редактор стилей](https://styles.2gis.com/) карты 2gis и [документация](https://docs.2gis.com/ru/mapgl/styles/overview)

## Исследование

1. [Тепловая карта плотности землетрясений](https://docs.mapbox.com/mapbox-gl-js/example/heatmap-layer/) на Mapbox
1. [Тепловая карта значений температуры](https://www.windy.com/-Temperature-temp?temp,54.902,83.034,5) на сервисе windy.com
1. Тепловые карты «плотности»

    - [Simpleheat](http://mourner.github.io/simpleheat/demo/)
    - [Heatmap.js](https://www.patrick-wied.at/static/heatmapjs/)
    - [WebGL Heatmap](https://github.com/pyalot/webgl-heatmap)
    - [Mapbox Heatmap](https://docs.mapbox.com/mapbox-gl-js/example/heatmap-layer/)
    - [Heatmapper](http://www.heatmapper.ca/geocoordinate/) на [R](<https://ru.wikipedia.org/wiki/R_(%D1%8F%D0%B7%D1%8B%D0%BA_%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F)>)
    - [Алгоритм ядерной оценки плотности](https://ru.wikipedia.org/wiki/%D0%AF%D0%B4%D0%B5%D1%80%D0%BD%D0%B0%D1%8F_%D0%BE%D1%86%D0%B5%D0%BD%D0%BA%D0%B0_%D0%BF%D0%BB%D0%BE%D1%82%D0%BD%D0%BE%D1%81%D1%82%D0%B8)

1. Тепловые карты «значений»

    - [Temperature Map](https://github.com/optimisme/javascript-temperatureMap)
    - [Интерполяция на R](https://mgimond.github.io/Spatial/interpolation-in-r.html#idw)
    - [Алгоритм обратных взвешенных расстояний (IDW)](https://en.wikipedia.org/wiki/Inverse_distance_weighting)

## Реализация

1. [Алгоритм обратных взвешенных расстояний (IDW)](https://en.wikipedia.org/wiki/Inverse_distance_weighting)
1. Поиск объектов в пространстве

    - [RBush](https://github.com/mourner/rbush) и [R-дерево](<https://ru.wikipedia.org/wiki/R-%D0%B4%D0%B5%D1%80%D0%B5%D0%B2%D0%BE_(%D1%81%D1%82%D1%80%D1%83%D0%BA%D1%82%D1%83%D1%80%D0%B0_%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)>)
    - [Flatbush](https://github.com/mourner/flatbush) и [упакованное R-дерево Гильберта](https://en.wikipedia.org/wiki/Hilbert_R-tree#Packed_Hilbert_R-trees)
    - [KDBush](https://github.com/mourner/kdbush) и [K-мерное дерево](https://ru.wikipedia.org/wiki/K-d_%D0%B4%D0%B5%D1%80%D0%B5%D0%B2%D0%BE)

1. [d3-scale-chromatic](https://github.com/d3/d3-scale-chromatic#diverging) — цветовая палитра D3
1. Кластеризация

    - [Метод k-средних](https://ru.wikipedia.org/wiki/%D0%9C%D0%B5%D1%82%D0%BE%D0%B4_k-%D1%81%D1%80%D0%B5%D0%B4%D0%BD%D0%B8%D1%85)
    - [Библиотека skmeans](https://github.com/solzimer/skmeans#readme)

1. [d3-contour](https://github.com/d3/d3-contour#contourDensity) — контуры плотности данных D3
1. [geojson-vt](https://github.com/mapbox/geojson-vt) — разрезка гео-объектов на тайлы

## Результат

На данный момент тепловые карты стоимости аренды и продажи жилой недвижимости есть в следующих городах

-   [Новосибирск](https://2gis.ru/novosibirsk?layer=realty&sublayer=realtyPriceSale)
-   [Москва](https://2gis.ru/moscow?layer=realty&sublayer=realtyPriceSale)
-   [Санкт-Петербург](https://2gis.ru/spb?layer=realty&sublayer=realtyPriceSale)
-   [Кемерово](https://2gis.ru/kemerovo?m=86.08787%2C55.35999%2F12.38&layer=realty&sublayer=realtyPriceSale)
-   [Омск](https://2gis.ru/omsk?layer=realty&sublayer=realtyPriceSale)
-   [Красноярск](https://2gis.ru/krasnoyarsk?layer=realty&sublayer=realtyPriceSale)
-   [Екатеринбург](https://2gis.ru/ekaterinburg?layer=realty&sublayer=realtyPriceSale)
-   [Тюмень](https://2gis.ru/tyumen?m=65.539226%2C57.147579%2F12.16&layer=realty&sublayer=realtyPriceSale)
-   [Челябинск](https://2gis.ru/chelyabinsk?m=61.376987%2C55.156525%2F11.55&layer=realty&sublayer=realtyPriceSale)
-   [Краснодар](https://2gis.ru/krasnodar?m=39.000523%2C45.071472%2F11.6&layer=realty&sublayer=realtyPriceSale)
