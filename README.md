# custom-link-page

[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![HTML](https://img.shields.io/badge/HTML-5-orange)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS](https://img.shields.io/badge/CSS-3-blue)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

A customizable link-in-bio page built as a beginner coding project and commented to aid in my learning of HTML, CSS and JavaScript. Meant to replace a &#34;Linktree&#34; in an Instagram bio.

## Table of Contents

- [Install](#install)
- [Usage](#usage)
- [Maintainers](#maintainers)
- [Contributing](#contributing)
- [License](#license)

## Install
Open `index.html` in your browser — no build step or server needed.

## Usage
Visit the live page at [mezierenatalie.github.io/Custom-Link-Page](https://mezierenatalie.github.io/Custom-Link-Page/)

**To customize it for yourself:**

**Goodreads "currently reading" widget:**
- Open `currentlyreadingscript.js` and replace `GOODREADS_USER_ID` with your own Goodreads User ID
- Find your User ID in the URL after logging in: `https://www.goodreads.com/user/show/[YOUR_ID]`
- Your "currently reading" shelf must be set to public: Account Settings → Account & Notifications → Privacy → set profile to "anyone"

**Link buttons:**
- In `index.html`, update the `href` URL, favicon domain, and display text inside each link block

**Colors:**
- In `linkpagestyles.css`, update the hex codes in the `:root` block

**Features:**
- Auto-updating "currently reading" widget via Goodreads RSS
- Favicon icons pulled from linked sites automatically
- Responsive mobile layout

**How the widget works:**
The widget fetches your Goodreads "currently-reading" shelf RSS feed on every page load. Because browsers block direct requests to outside websites, the RSS URL is routed through [allorigins.win](https://allorigins.win), a free CORS proxy. The RSS response is parsed as XML, the most recently added book is extracted, and the title, author, and cover image are displayed in a styled card.

## Maintainers

[@Natalie Meziere](https://github.com/Natalie Meziere)

## Contributing
PRs are not accepted as this is a personal project, but feel free to fork it and make it your own!


Small note: If editing the README, please conform to the
[standard-readme](https://github.com/RichardLitt/standard-readme) specification.

## License

MIT © 2026 Natalie Meziere
