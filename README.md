5. По умолчанию выделено:
- 2 логических процессора 
- 1024 Мб оперативной памяти 
- Жёсткий диск на 64 Гб
- Графический контроллер VBoxVGA с 4 Мб оперативной памяти
- оптический диск
- 1Гб/с сетевая карта 
6. Изменить количество выделенной оперативной памяти и ресурсов процессора можно с помощью кода в Vagrantfile:
``` 
config.vm.provider "virtualbox" do |v|
	  	v.memory = 2048
  		v.cpus = 3
end
```

8. 
- Переменная HISTSIZE (595 строчка мануала)
- ignoreboth не записывает в историю пробелы перед командами, а также последняя команда, если она ещё раз вызвана
9. Строка 746. Могут быть использованы для генерирования произвольных строк. Этот механизм аналогичен расширению имени пути, но сгенерированные имена файлов могут не существовать. Шаблоны, которые должны быть расширены фигурными скобками, принимают форму необязательной преамбулы, за которой следует либо ряд строк, разделенных запятыми, либо выражение последовательности между парой фигурных скобок, за которым следует необязательный постскриптум. Также может использоваться для описания последовательности от x к у с шагом incr в формате {x..y[..incr]}, где х и y, incr (опциональный параметр) - целые числа.
10. Создать 100 000 файлоов одной командой: 
`touch {1..100000}`.
Для добавления 300 000 файлов нужно расширить буфер linux (`ulimit -s 24576`), так как количество аргусентов для команды превышает его затем файлы можно создать `touch {1..300000}`
11. `[[ -d /tmp ]]` возвращает `true`, если директория `/tmp` существует, `false`, если не существует
12.  
```
$cd /tmp
$mkdir new_path_directory
$cd new_path_directory/
$cp /usr/bin/bash /tmp/new_path_directory/bash
$type -a bash
bash is /tmp/new_path_directory/bash
bash is /usr/bin/bash
bash is /bin/bash
 ```
 13. Задания at можно запланировать на определённое время в будущем, а задания batch будут выполнены в будущем не по времени, а когда средняя нагрузка станет меньше 1,5
