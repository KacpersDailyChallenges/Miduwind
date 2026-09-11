<a id="readme-top"></a>

<div align="center">

![Astro](https://astro.build/assets/press/astro-icon-light-gradient.svg)

[![Available at](https://img.shields.io/badge/Available%20at-Astro%20Themes-purple?style=for-the-badge&link=https://astro.build/themes/details/astrolinkhub/)](https://astro.build/themes/details/miduwind/)

</div>

<h1 align="center">Miduwind</h1>

<div align="center">

![Astro](https://img.shields.io/badge/Astro-0C1222?style=for-the-badge&logo=astro&logoColor=FDFDFE)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![JSON](https://img.shields.io/badge/json-5E5C5C?style=for-the-badge&logo=json&logoColor=white)

Open source links page, customizable via JSON. Made with Astro 5 and Tailwind 4.

</div>

![Screenshot](/public/screenshot.png)

## Table of Contents

  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li>
      <a href="#json">JSON</a>
    </li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
  </ol>

## About The Project

While looking for a clean way to build my own link-in-bio page, I came across
[Miduwind](https://github.com/MarcosKlender/Miduwind) — an open-source template
created by [MarcosKlender](https://marcosklender.com) — and honestly thought it
was a fantastic piece of work: modern, polished, and refreshingly easy to
customize through a single JSON file. It's exactly the kind of template that
made me want to fork it rather than start from scratch.

So I did — I forked Miduwind and adapted it into my own personal links page for
**Kacpers Daily Challenges**, tweaking the design and adding a few features
along the way (see [Credits](#credits) for the full list of changes):

- Built with Astro (v5.7) and Tailwind (v4.1)
- Fully customizable via a single `data.json` file
- Free and open source — feel free to fork it too!

## Getting Started

### Prerequisites

- **Node.js** -> `v18.17.1` or `v20.3.0` or higher. (`v19` is not supported)
- **Visual Studio Code** -> with the [Official Astro Extension](https://marketplace.visualstudio.com/items?itemName=astro-build.astro-vscode).

Personally I prefer using `pnpm` instead `npm` and to install it you can use:

```sh
npm install -g pnpm
```

### Installation

1. Clone this repo to your computer:
   ```sh
   git clone git@github.com:KacpersDailyChallenges/Miduwind.git
   ```
2. Install Astro dependencies:
   ```sh
   cd Miduwind
   pnpm install
   ```
3. Run the Astro dev server:
   ```sh
   pnpm dev
   ```

<p align="right"><a href="#readme-top">Back to top ⬆️</a></p>

## JSON

The best part of Miduwind is that you can modify every aspect of the website very easily, you just have to edit the `data.json` file. This JSON contains the following sections:

- **html** -> Edit language, title, description, favicon (replace it in `/public`) and the page gradient background.
- **header** -> Edit your photo (replace it in `/public`) and your username.
- **about** -> Edit your name and a summary about you.
- **links** -> Highlight your links with a gradient background and a logo.
- **footer** -> Edit the copyright and URL of your choice (Made just for you 😎).

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "feature".
**Don't forget to give the project a star!** ⭐

<p align="right"><a href="#readme-top">Back to top ⬆️</a></p>

## Credits

Based on [Miduwind](https://github.com/MarcosKlender/Miduwind) by MarcosKlender (MIT License).

Modified by KacperDailyChallenges:
- **Redesigned profile header** – circular avatar with an accent-colored glow and a
  username badge anchored to the bottom edge (previously a plain photo with a label
  overlapping the top).
- **Fully dynamic links grid** – any number of links now render automatically in
  rows, alternating between 2:1 and 1:2 tile proportions (previously hardcoded to
  exactly six links).
- **Configurable tile icons** – icon size and offset from the tile edge are now set
  globally via `globalSettings` in `data.json`, replacing the previous fixed
  rotate-on-hover animation.
- **Multi-entry footer** – the footer now supports a list of credit links instead of
  a single one, used here to credit both the original author and this fork.
- **Smoother responsive scaling** – layout width and grid breakpoints scale more
  gradually across screen sizes instead of jumping at fixed breakpoints (e.g. tiles
  switch from one to two columns around 400px instead of 768px, and the page uses a
  fluid width with a max cap instead of stepped widths).
- **Official brand icons** – swapped generic SVG icons for each platform's official
  logo assets.
- **Minor UI polish** – more compact tiles, a stable scrollbar gutter to prevent
  layout shift, and a placeholder "separator" tile.

This fork also adds an explicit `LICENSE.txt` to formalize the MIT terms referenced
above, and adapts all descriptions/links/colors to KacperDailyChallenges' own
socials.

<p align="right"><a href="#readme-top">Back to top ⬆️</a></p>

## License

Distributed under the MIT License. `Open Source` is pretty self-descriptive.

<p align="right"><a href="#readme-top">Back to top ⬆️</a></p>
