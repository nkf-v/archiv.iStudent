# archivy.iStudent

Для кодирования и декодирования применяется статический класс Archivy.

Этот класс содержит два метода `Compress(nameFile)` и `Decompress(nameFile)`
Где `nameFile` это имя файла который.

Метод `Compress` кодирует файл и форматирует его в `.sz`.
Метод `Decompress` декодирует файл формата `.sz` убирает из имени файла формат `.sz` и приписывает приставку `copy` чтобы небыло переписывания оригинального файла если тот присутствует в той же папке где и передоваемый файл.

Пример использование класса:

```C#
static void Main(string[] args)
{
	string nameFile = Console.ReadLine();
	Archivy.Compress(nameFile);
}
```
<!-- Для запуска архиватора перейдите в папку `bin/Debug`
и через консоль введите команду:

`$ ConsoleApplicationArchivy <mode> [Files, ]`

Где `<mode>` режим архиватора:

1. `--com` архиваирование файлов
2. `--uncom` деархиваирование файлов

`[Files, ]` имена файлов которые вы хотите архивировать или деархивировать:

Пример `ConsoleApplicationArchivy --com input.txt output.txt`

В данном пример будуд архивироваться два файла `input.txt` и `output.txt`.
По окончанию программы в той же директории будудт два файла `input.txt.sz` и `output.txt.sz`. -->