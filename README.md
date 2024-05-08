# Lab2 RISC-V
## Задание (вариант 9)
Вид исключения: Environment call from M-mode
Тест: isa/rv32mi/scall.S
Reset vector: 0x800
Trap vector: 0x400
Обработчик: Вывод строки «Detect envcall from M-mode»

## Ход выполнения
1) Отредактирован список тестов в файле **rv32_tests.inc**, оставлен только тест **isa/rv32mi/scall.S**.
2) Модифицированы вектора прерываний и ресетов в процессоре (файл **scr1_arch_description.svh**).
3) Откорректированы смещения в файлах **link.ld** и **riscv_macros.h**. В заголовочный файл добавлен **.text.start** по адресу 0x800.

## Результаты выполнения работы
+ ./results/trace.log - трейслог
+ ./results/test_results.txt - результат симуляции
+ ./results/scall.dump - файл, содержащий дизассемблер теста

## Результаты проверки теста
Результаты прохождения теста в терминале:  
![image](https://github.com/TimesNewRomanHub/scr1/assets/159648521/fdfd3324-f18f-448c-927a-41dad87f238f)  

Графики вейвформ (Reset vector = 0x800, Trap vector = 0x400)  
![image](https://github.com/TimesNewRomanHub/scr1/assets/159648521/18856c6e-54ad-4f55-ac9c-ce0128cfaea9)

