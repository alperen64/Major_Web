# Major Pub

A responsive pub website with a multilingual menu, an events calendar and a browser-local reservation demonstration. Built with plain HTML, CSS and JavaScript.

## Features

- Turkish, English and Bulgarian interface text
- Menu categories and product prices
- Event browsing and date selection
- Local reservation creation, approval and removal
- Local menu and event editing controls

## Run locally

Open `Major Web/Major Pub Web.html` in a browser. For an HTTP preview, run `python -m http.server 8080` inside `Major Web/`, then visit `http://localhost:8080/Major%20Pub%20Web.html`.

No installation or build step is required. Fonts and the remote logo require an internet connection.

## Project structure

```text
Major Web/
  Major Pub Web.html   Self-contained application
  css                 Separate copy of the inline stylesheet
  script              Separate copy of the inline script
```

The HTML is the runnable entry point. It does not import the two extensionless copies. Keep the inline script and its separate copy synchronized when changing behavior.

## Data and deployment

Data is stored under `majorPubDB_v10` in the current browser's `localStorage`. Reservations are not sent to the venue or synchronized between devices. The local administrator controls are a UI demonstration, not server-side authentication. Do not use this version to collect real customer reservations on a shared device.

For a public static preview, host the HTML as the entry point. Real reservation delivery and shared administration require a backend with authenticated access, input validation and appropriate personal-data handling.

## Assets

Venue branding and linked third-party resources retain their respective ownership. No license granting reuse is declared in this repository.
