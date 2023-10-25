Лабораторная работа №1


Внимание! В связи с поздним опубликованием лабораторной работы, вторая часть лабораторной работы (реальный бенчмарк) удалена из задания.

Основная цель лабораторной работы — знакомство с системными инструментами анализа производительности и поведения программ. 
В данной лабораторной работе Вам будет предложено произвести нагрузочное тестирование Вашей операционной системы при помощи инструмента stress-ng.

В качестве тестируемых подсистем использовать: cpu, cache, io, memory, network, pipe, scheduler.

Для работы со счетчиками ядра использовать все утилиты, которые были рассмотренны на лекции (раздел 1.9, кроме kdb)

Ниже приведены списки параметров для различных подсистем (Вам будет выдано 2 значения для каждой подсистемы согласно варианту в журнале). 
Подбирая числовые значения для выданных параметров, и используя средства мониторинга, добиться максимальной производительности системы (BOGOPS, FLOPS, Read/Write Speed, Network Speed).

Построить графики (подходящие по заданию.):

Потребления программой CPU;
Нагрузки, генерируемой программой на подсистему ввода-вывода;
Нагрузки, генерируемой программой на сетевую подсистему;
Другие графики, необходимые для демонстрации работы.

Мой вариант:
cpu: [phi,union]; 
cache: [l1cache-ssize,cache-level];
io: [ioport,iomix]; 
memory: [misaligned-method,mmaphuge-mmaps]; 
network: [netdev,netlink-task]; 
pipe: [pipe-data-size,pipe-size]; 
sched: [resched,sched-period]