# Shivam Singhania — Official Telegram Channel

A single-page landing site that introduces the Shivam Singhania Telegram channel, shows a few headline stats, and links visitors to the channel with a prominent join button. A 15-second countdown ring under the button redirects visitors to Telegram automatically.

## Technologies

- Plain HTML, CSS, and vanilla JavaScript (no build step)
- Google Fonts (Cinzel, Montserrat) and Font Awesome icons via CDN
- Hosted on Netlify as a static site

## Running locally

Open `public/index.html` in a browser, or serve it with any static server, for example:

```bash
npx serve public
```

## Editing

- Telegram link: update both the button `href` and the `TELEGRAM_URL` constant in `public/index.html`.
- Countdown length: change `timeLeft` and `totalTime` in the script block.
