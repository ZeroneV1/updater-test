# Text File Formatting and Fetch Locations for News and Changelog

Your `news.txt` and `changelog.txt` files support special syntax for formatting text and creating links within the undergr0und application. This document also explains where in the code you can change the locations from which these files are fetched.

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

## Changing Text File Fetch Locations

The URLs from which the `news.txt` and `changelog.txt` files are fetched are specified directly in the JavaScript code within your `Launcher.html` file.

To change these locations:

1.  Open your `Launcher.html` file in a text editor.
2.  Find the `fetchNews()` JavaScript function. Locate the `fetch()` call within this function:
    ```javascript
           fetch('[https://hostfilez.glitch.me/news.txt](https://hostfilez.glitch.me/news.txt)')
    ```
    Replace `'https://hostfilez.glitch.me/news.txt'` with the new URL for your `news.txt` file.
3.  Find the `openChangelogModal()` JavaScript function. Locate the `fetch()` call within this function:
    ```javascript
           fetch('[https://hostfilez.glitch.me/changelog.txt](https://hostfilez.glitch.me/changelog.txt)')
    ```
    Replace `'https://hostfilez.glitch.me/changelog.txt'` with the new URL for your `changelog.txt` file.

Ensure that the new URLs you provide are publicly accessible via HTTP or HTTPS.
