# Билет №1.9 Схема Бернулли.

## Формулировка

***Определения:***
Для применения схемы Бернулли должны быть выполнены следующие условия:
1. Каждое испытание имеет ровно два исхода (успех и неудача)
2. Независимость испытаний: результат очередного эксперимента не должен зависеть от результатов предыдущих экспериментов.  
3. Вероятность случайных событий $A$ неизменна для всех испытаний:
$P(A) = p$ - const
4. Количество $n$ испытаний - конечно

Такая схема испытаний называется ***схема Бернулли***

***Теорема:*** Пусть вероятность, что в отдельном опыте произойдет событие $A$, равна p. Тогда вероятность, что в $n$ независимых опытах $m$ раз случится $A$:

$\displaystyle P_n(m) = C^m_n p^m(1-p)^{n-m} = \frac{n!}{m!(n-m)!}p^m(1-p)^{n-m}$

***Доказательство:***  

$A$ - случившееся событие  
$n$ - количество независимых опытов  
$m$ - количество случившихся $A$  
$p$ - вероятность $A$  
$q = 1 - p$ - вероятность, что $A$ не произойдет

Пусть событие, что $A$ произошло $m$ раз и не произошло $n-m$: $A * A * ... * A * \bar A * ... * \bar A$  
\*тут $A$ всего $m$, а 
$\bar A$ всего $n-m$\*

Из независимости случайных событий можно применить правило вычисления вероятности произведения независимых событий:  
$P(A * A * ... * A * \bar A * ... * \bar A) = p^mq^{n-m}$

Но тк последовательность $A$ и 
$\bar A$ может измениться, то количество сочетаний найдем как $C^m_n$

И тогда: $P_n(m) = C^m_np^m(1-p)^{n-m}$ - ***биномиальная схема Бернулли***

## Частные случаи

$\displaystyle P_n(n)=\frac{n!}{n!*0!} = p^n$

$P_n(0)=q^n$

## Пример

***Дано:*** Вероятность попадания в цель - 0.8. Найти вероятность 4 попаданий из 6 выстрелов.

***Решение:*** $n = 6, m = 4, p = 0.8, q = 0.2$   

$\displaystyle P_6(4) = C^m_np^mq^{n-m} = C^4_60.8^40.2^{6-4} = \frac{6!}{4!2!}0.8^40.2^2 = 0.24576$

***Ответ:*** 0.24576

---
## Создатель

Автор расписанного билета: Алиса Хайдарова

Кто проверил:
- Квист Татьяна

## Ресурсы
- лекции