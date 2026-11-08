# Axiom Verge — українська локалізація

Неофіційний українізатор для **Axiom Verge (2015)**.

## Windows 64-bit: встановлення без додаткового ПЗ

[Завантажити готовий ZIP](https://github.com/SmailWolf/AxiomVerge-UA/releases/download/v1.1.0/AxiomVerge-UA-Windows-1click-v1.1.0.zip).

1. Розпакуй ZIP повністю.
2. Двічі клацни Install-AxiomVerge-UA.bat.
3. Вибери папку гри з AxiomVerge.exe і підтверди встановлення.

Окремо встановлювати Node.js або Python та підключатися до інтернету не потрібно. ZIP містить переносні версії потрібних компонентів. Файл .bat запускає сценарій .ps1 у Windows PowerShell; обидва призначені для Windows. Оригінальні файли зберігаються в папці Axiom Verge UA backup. Щоб відновити їх, запусти Restore-AxiomVerge-UA.bat.

Патчер підтримує лише перевірену версію гри. Файли самої гри не розповсюджуються.

## Linux

Windows .bat і .ps1 файли в Linux не запускаються. Для Linux потрібні Node.js, npm, Python 3 і pip. Завантаж вихідний архів AxiomVerge-UA-source-v1.zip з репозиторію, розпакуй його та з папки проєкту виконай:

```sh
npm install
python3 -m pip install --user -r requirements.txt
npm run patch -- '/шлях/до/Axiom Verge'
```

Команда створить файли патча в build/Axiom Verge UA patch у папці гри. Перед ручною заміною збережи оригінали.

## Переклад і безпека

Переклад охоплює 841 текстовий запис і 19 елементів титрів. Повне проходження гри для редакторської вичитки ще не виконано.

Новий Windows ZIP з переносними компонентами ще не сканувався VirusTotal. Попередній вихідний архів отримав 0 із 66 виявлень, але це інший файл: [звіт VirusTotal](https://www.virustotal.com/gui/file-analysis/YzdmNWI3YTdmMzUwZDc0YjM1ZTMwNTE5NjBmZWZlMzE6MTc5NDE0NjY1Ng==). Результат попереднього сканування не поширюється на новий ZIP і не гарантує повної безпеки.
