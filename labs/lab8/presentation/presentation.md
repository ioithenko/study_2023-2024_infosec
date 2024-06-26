---
## Front matter
lang: ru-RU
title: Лабораторная работа №8
subtitle: Основы информационной безопасности
author:
  - Ищенко Ирина
institute:
  - Российский университет дружбы народов, Москва, Россия


## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Ищенко Ирина Олеговна
  * НПИбд-02-22


:::
::: {.column width="30%"}


:::
::::::::::::::

## Цель работы

Освоить на практике применение режима однократного гаммирования
на примере кодирования различных исходных текстов одним ключом.

# Выполнение лабораторной работы

## Функция

```python
def encrypt(text: str, key: list = None):
    if not key:
        key = generate_key(length=len(text))

    text_16 = [ord(char) for char in text]    
    key = [ord(el) for el in key]

    print(f"Ключ шифрования:", ' '.join(str(s) for s in key))
    print(f"Исходный текст:", text)
    
```

## Функция


```python
    encrypted_text = []
    for i in range(len(text)):
        encrypted_text.append(text_16[i] ^ key[i])

    ciphertext = ''.join([chr(i) for i in encrypted_text])
    print(f'Шифротекст: {ciphertext}\n\n')

    return ciphertext
 ```  


## Реализация


```python
p1 = 'НаВашисходящийот1204'
p2 = 'ВСеверныйфилиалБанка'
key = generate_key(20)

c1 = encrypt(p1, key=key)
c2 = encrypt(p2, key=key)

c1_c2 = encrypt(c1, key=c2)

encrypt(c1_c2, p1)
encrypt(c1_c2, p2)
```


## Выполнение

![Вывод программы](image/1.png){#fig:001 width=45%}


## Выводы

В ходе выполнения лабораторной работы я освоила на практике применение режима однократного гаммирования на примере кодирования различных исходных текстов одним ключом.
