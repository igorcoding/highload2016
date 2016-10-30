class:firstpage

# Отказоустойчивая обработка 10 миллионов<br> OAuth токенов на Tarantool 

### Mons Anderson<br>Игорь Латкин

---
layout: true
class: center, middle

---

# оптимальность

---

# винил

---

# json документы

---

# What else&hellip;

---

# Failover!

---
layout: false

# The road so far

--

## Что было 3 года назад?

--

## Какие проблемы были?

--

## Master ⟷ Master репликация

--

## В поисках Raft'а

--

## Объединяем Raft и шардинг

--

## Оцениваем результат

---

# 2013

\[ F ⇾ M ⇽ Ref ] \[ F ⇾ S ⇽ Ref ]

---

# Зачем?

## Сборщики почты
## Вход внешней почтой
## Хранение адресных книг
## Выдача действующего access_token

---

# Что такое OAuth токен?
.big[
```json
{
    "token_type"    : "bearer",
    "access_token"  : "XXXXXX",
    "refresh_token" : "YYYYYY",
    "expires_in"    : "3600"
}
```
]

---

# Что такое OAuth токен?
.big[
```json
{
    "token_type"    : "bearer",
    "access_token"  : "XXXXXX",
    "refresh_token" : "YYYYYY",
*   "expires_in"    : "3600"
}
```
]

---

# Проблемы?

100% Outage за 1 час

---
class: image-text

.svg[![sample image](raft-base.svg)]

---
class: h-margin, center, middle

.right[
![image](tarantool1.svg)
]

## Get your<br> data in RAM
## .red[Compute<br> close to data]
## Enjoy the<br> performance

---

.right[
## [tarantool.org](http://tarantool.org/doc)
]
.left[
## Documentation:
]
.right[
##[try.tarantool.org](http://tarantool.org/doc)
]
.left[
## Try it online: 
]

.right[
##[github.com/tarantool](http://github.com/tarantool)
]
.left[
## Explore it: 
]

.right[
##[github.com/mons/tnt-luas](http://github.com/mons/tnt-luas)
]
.left[
## Luas: 
]

.smallimg[
![image](tarantool1.svg)
]

.lastquote[
### Questions?
]
