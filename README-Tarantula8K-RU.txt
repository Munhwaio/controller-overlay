GameSir Tarantula 8K — Dark Neon Edition
Пакет для GamePad Viewer, база: PlayStation 4 (White), skin s=8.

Содержимое:
- tarantula8k-dark-neon.css — таблица стилей для поля Edit CSS URL.
- tarantula8k-dark-neon-base.png — прозрачный графический слой корпуса.

Установка:
1. Разместите оба файла в одной папке публичного статического хостинга.
   Подойдёт публичный GitHub-репозиторий с GitHub Pages или другой хостинг,
   который отдаёт CSS/PNG без авторизации и разрешает cross-origin загрузку.
2. Скопируйте прямую HTTPS-ссылку на tarantula8k-dark-neon.css.
3. Откройте сохранённый контроллер GamePad Viewer: https://beta.gamepadviewer.com/gamepads/y5LXjT4Cs1
4. Нажмите Edit, оставьте Skin = PlayStation 4 (White), поле Edit CSS URL заполните прямой ссылкой на CSS.
5. Нажмите Save, откройте overlay и подключите контроллер по USB. Нажмите любую кнопку для активации Gamepad API.

Важно:
- CSS использует известную DOM-структуру DS4/PS4-кожи GamePad Viewer: .controller, .triggers,
  .trigger, .bumpers, .bumper, .abxy, .button, .sticks, .stick, .dpad, .face, .meta.
- Твои HTML-сохранения содержат страницу настроек, но не содержат внутреннюю разметку iframe с рендером контроллера.
  Поэтому это стартовая интеграция под подтверждённую skin s=8 и стандартные DS4-классы, а не результат live-проверки.
- После подключения нужно проверить центровку слоёв в живом preview. Если конкретная сборка Beta использует другие классы
  либо DOM-порядок отличается, CSS потребуется скорректировать по Inspect внутри iframe.
