# undergr0und - Web Game Launcher & Viewer

undergr0und is a custom web-based application designed to provide a simple and accessible platform for launching and viewing online games and websites, with a focus on circumventing internet censorship. It features a clean interface, a built-in viewer, a personalized library for favorites, and customizable themes.

## Features

* **Game Launcher:** Easily access a curated list of web games.
* **Integrated Viewer:** Play games and browse websites directly within the app using an iframe overlay.
* **Proxy Support:** (Where configured for specific games/sites) Access blocked content via a built-in proxy mechanism.
* **Personal Library:** Save your favorite games and websites to a dedicated library.
* **Recently Viewed:** Keep track of the websites and games you've recently accessed.
* **Customizable Themes:** Personalize the app's appearance with different color themes.
* **Dynamic News Feed:** Stay updated with news fetched from an external source.
* **Changelog:** View recent updates and changes to the application.
* **Drag and Drop:** Reorder games on the Games page using drag and drop.
* **Add Custom Games:** Easily add new web games to your launcher.

## How to Use

1.  Open the `Launcher.html` file in a modern web browser.
2.  Navigate through the different sections using the sidebar icons (Home, Library, Viewer, Games, Updater, Settings, About).
3.  On the **Home** page, you can see the Game of the Day and the latest news. Use the search bar to quickly launch a URL in the viewer.
4.  On the **Games** page, click on a game card to launch it in the viewer. You can add games, favorite them, toggle proxy (if available), and reorder them by dragging and dropping.
5.  The **Library** page shows your favorited websites/games and your recently viewed history.
6.  Use the **Viewer** icon to open the viewer overlay directly to input a URL.
7.  In **Settings**, you can change the application's theme and reset your saved data.
8.  The **About** page provides information about the application and credits.
9.  Click the **Changelog** button (available on Home and About pages) to see the update history.

## Setup and Hosting

To get undergr0und up and running, you need to host the `Launcher.html` file and ensure the external news and changelog files are accessible.

1.  **Host the `Launcher.html` file:** You can host this file on any web server. Simple options include:
    * **GitHub Pages:** If your code is on GitHub, you can easily host the HTML file directly from a repository branch (e.g., `gh-pages` branch or the `main`/`master` branch's docs folder).
    * **Glitch:** You can host the HTML file and your `news.txt` and `changelog.txt` files together on a service like Glitch.
    * **Any Static Web Host:** Upload the file to a service that hosts static HTML files.
2.  **External Files (`news.txt` and `changelog.txt`):** The application fetches news from `https://hostfilez.glitch.me/news.txt` and the changelog from `https://hostfilez.glitch.me/changelog.txt`.
    * Ensure these files exist at the specified URLs. You can host them on the same service as your `Launcher.html` or a different one, as long as they are publicly accessible via HTTP/HTTPS.
    * Modify the content of these `.txt` files on your hosting service to update the news feed and changelog in your application.

## Technologies Used

* **HTML, CSS, JavaScript:** The core web technologies.
* **Vanta.js:** For the animated background effects (uses Three.js).
* **Three.js:** A 3D JavaScript library used by Vanta.js.
* **Font Awesome:** For icons.
* **localStorage:** For saving user data locally (games list, library, favorites, theme).
* **Fetch API:** For fetching external news and changelog files.

## Credits

* Created by: Zerone
* Backgrounds: Vanta.js, Three.js.
* Icons: Font Awesome.

## License
Copyright (c) [2025] [zerone.v1]

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
