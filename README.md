# ChessGameConsole
Игра в шахматы. По координатам шахматной доски. Случайна генерация хода по нажатию клавиши Enter.

Скачать программу в архиве (Release версия):
https://drive.google.com/file/d/1ceCdpIVzkvz7JEVipFjp60wTfMv7cOpl/view?usp=sharing

Если не делать (не вводить) ходы, а просто нажимать 'Enter', ходы будут генерироваться случайным образом, но по шахматным правилам.

Чтобы сделать ход нужно ввести например - "Pe2e4" - "ход белой пешки с Е2 на Е4" и т.д.

В Visual Studio: Решение "GeneralShessClassLibrary". Рабочая среда ".NET Framework". 

Библиотека классов 'GameChess'.
A. 'GameShess' (namespace GameShess):

	1. // 1-м создаю общий класс GameShess.ChessClass - "public class ChessClass";
	2. // 3-м создаю перечисление (класс) шахматных фигур - "enum ChessFigures";
	3. // 4-м создаю перечисление для цвета игрока - "enum ColorPlayer"
	4. // 5-ой создаю структуру шахматных клеток на доске - "struct SquareBoard";
	5. // 6-й создаю класс 'фигура на клетке' - "class FigureOnSquare";
	6. // 7-й создаю класс 'фигура делает ход' - "class FigureMoving";
	7. // 8-м делаю класс для шахматной доски - "class ChessBoard";
	8. // 9-й класс для движений фигур - "class ChessMoves";

Тип выходных данных "Консольное приложение".
B. 'ConsoleChess' (namespace ConsoleChess; файл: ProgramChess.cs)

	1. // 2-й создаю консоль - "class ProgramChess" (namespace ConsoleChess).

Прочие настройки:
Для консоли установить шрифт "Lucida Console" размер: 20.
Для игры с компьютером - генератор случайных чисел - по нажатию Enter.
Для вывода на экран - шахматы в ASCII формате.
Для работы с цветом: 'ForegroundColor' - возвращает или задает цвет фона консоли.

Фэн-параметры беру с - https://en.wikipedia.org/wiki/Forsyth%E2%80%93Edwards_Notation

Редактор шахматной доски представлен на: https://lichess.org/editor

Начальная позиция фигур на доске: string fen = "rnbqkbnr/pppppppp/8/8/8/8/PPPPPPPP/RNBQKBNR w KQkq - 0 1"
