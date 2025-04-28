# Text File Formatting for News and Changelog

Your `news.txt` and `changelog.txt` files support special syntax for formatting text and creating links within the undergr0und application.

## General Formatting (News and Changelog)

The following syntax can be used in both `news.txt` and `changelog.txt`:

* **Links to App Pages:** To create a link that navigates to a specific page within the undergr0und app, use semicolons around the page name:
    `;PageName;`
    Replace `PageName` with the exact name of the page (e.g., `Home`, `Library`, `Viewer`, `Games`, `Updater`, `Settings`, `About`).
    *Example:* `Check out the ;Games; page!` will create a link to the Games page.

* **Text Size:** To change the size of a block of text, use double square brackets with `size:` followed by the size value (e.g., `1.5em`, `24px`) before the text, and `[[/size]]` after the text:
    `[[size:size]]Your text here[[/size]]`
    *Example:* `[[size:1.2em]]Important Announcement[[/size]]`

* **Bold Text:** To make text bold, wrap it in double asterisks:
    `**Your bold text here**`
    *Example:* `**New Feature Added!**`

* **Italic Text:** To make text italic, wrap it in single asterisks:
    `*Your italic text here*`
    *Example:* `*This is a note.*`

* **Line Breaks:** Standard line breaks (pressing Enter) in your `.txt` file will be preserved.

## Special Syntax (News Only)

* **Game of the Day:** In your `news.txt` file, you can designate a "Game of the Day" by including the exact name of a game from your `games` array within curly braces `{}`. This marker will be removed from the news text itself, and the specified game will be featured separately.
    `{Exact Game Name}`
    *Example:* If you have a game named "Agar.io" in your games list, including `{Agar.io}` in your `news.txt` will set it as the Game of the Day.

Remember to save your `.txt` files with plain text encoding (like UTF-8) when updating them on your hosting service.
