# AstroPaper | Modèle de Blog avec Pages CMS📄

![AstroPaper](public/astropaper-og.jpg)
![Typescript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![GitHub](https://img.shields.io/github/license/satnaing/astro-paper?color=%232F3741&style=for-the-badge)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white&style=for-the-badge)](https://conventionalcommits.org)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg?style=for-the-badge)](http://commitizen.github.io/cz-cli/)

AstroPaper est un thème de blog minimal, responsive, accessible & SEO-friendly. Ce thème est conçu et personalisé sur la base du [blog de satnaing](https://satnaing.dev/blog).

Ce thème suit les bonnes pratiques et fournis une accessibilité complète. Il support par défaut les modes Light & Dark. De plus, des palettes de couleurs additionnelles peuvent être configurée.

Ce thème est autodocumenté \_ ce qui signifie que les articles/posts peuvent également être considéré comme de la documentation. Lisez [l'article de blog](https://astro-paper.pages.dev/posts/) ou [La section Lisez-Moi](#-documentation) pour plus d'information.

## 🔥 Fonctionalités

- [x] type-safe markdown
- [x] super fast performance
- [x] accessible (Keyboard/VoiceOver)
- [x] responsive (mobile ~ desktops)
- [x] SEO-friendly
- [x] light & dark mode
- [x] fuzzy search
- [x] draft posts & pagination
- [x] sitemap & rss feed
- [x] followed best practices
- [x] highly customizable
- [x] dynamic OG image generation for blog posts [#15](https://github.com/satnaing/astro-paper/pull/15) ([Blog Post](https://astro-paper.pages.dev/posts/dynamic-og-image-generation-in-astropaper-blog-posts/))

_Note: La fonction d'accessibilité de lecture d'écran AstroPaper utilisant **VoiceOver** sur MAC et **TalkBack** sur Android ont été testés. 

## ✅ Lighthouse Score

<p align="center">
  <a href="https://pagespeed.web.dev/report?url=https%3A%2F%2Fastro-paper.pages.dev%2F&form_factor=desktop">
    <img width="710" alt="AstroPaper Lighthouse Score" src="AstroPaper-lighthouse-score.svg">
  <a>
</p>

## 🚀 Project Structure

A l'intérieur d'AstroPaper, voici l'arborescence de répertoires et fichiers :

```bash
/
├── public/
│   ├── assets/
│   │   └── logo.svg
│   │   └── logo.png
│   └── favicon.svg
│   └── astropaper-og.jpg
│   └── robots.txt
│   └── toggle-theme.js
├── src/
│   ├── assets/
│   │   └── socialIcons.ts
│   ├── components/
│   ├── content/
│   │   |  blog/
│   │   |    └── some-blog-posts.md
│   │   └── config.ts
│   ├── layouts/
│   └── pages/
│   └── styles/
│   └── utils/
│   └── config.ts
│   └── types.ts
└── package.json
```

Astro cherche les fichiers `.astro` ou `.md` dans le répertoire `src/pages/`. Chaque page est exposée en tant que route avec son propre nom.

Tous les composants statiques, comme les images, peuvent être ajoutés dans le répertoire `public/`.

Tous les articles peuvent être stocké dans le répertoire `src/content/blog`.

## 📖 Documentation

Documentation peut être lue dans deux formats\_ _markdown_ & _blog post_.

- Configuration - [markdown](src/content/blog/how-to-configure-astropaper-theme.md) | [blog post](https://astro-paper.pages.dev/posts/how-to-configure-astropaper-theme/)
- Ajouter des articles - [markdown](src/content/blog/adding-new-post.md) | [blog post](https://astro-paper.pages.dev/posts/adding-new-posts-in-astropaper-theme/)
- Personnaliser la palette de couleurs - [markdown](src/content/blog/customizing-astropaper-theme-color-schemes.md) | [blog post](https://astro-paper.pages.dev/posts/customizing-astropaper-theme-color-schemes/)
- Palettes de couleurs prédéfinies - [markdown](src/content/blog/predefined-color-schemes.md) | [blog post](https://astro-paper.pages.dev/posts/predefined-color-schemes/)

> Pour AstroPaper v1, jetez un oeil à [cette branche](https://github.com/satnaing/astro-paper/tree/astro-paper-v1) et cette [URL](https://astro-paper-v1.astro-paper.pages.dev/)

## 💻 Tech Stack

**Main Framework** - [Astro](https://astro.build/)  
**Type Checking** - [TypeScript](https://www.typescriptlang.org/)  
**Component Framework** - [ReactJS](https://reactjs.org/)  
**Styling** - [TailwindCSS](https://tailwindcss.com/)  
**UI/UX** - [Figma](https://figma.com)  
**Fuzzy Search** - [FuseJS](https://fusejs.io/)  
**Icons** - [Boxicons](https://boxicons.com/) | [Tablers](https://tabler-icons.io/)  
**Code Formatting** - [Prettier](https://prettier.io/)  
**Deployment** - [Cloudflare Pages](https://pages.cloudflare.com/)  
**Illustration in About Page** - [https://freesvgillustration.com](https://freesvgillustration.com/)  
**Linting** - [ESLint](https://eslint.org)

## 👨🏻‍💻 Running Locally

Le moyen le plus simple d'exécuter ce projet localement est d'exécuter la commande suivante dans le répertoire souhaité.

```bash
# npm 6.x
npm create astro@latest --template satnaing/astro-paper

# npm 7+, extra double-dash is needed:
npm create astro@latest -- --template satnaing/astro-paper

# yarn
yarn create astro --template satnaing/astro-paper
```

## Google Site Verification (optional)

Vous pouvez ajouter votre [Tag Google Site Verification HTML](https://support.google.com/webmasters/answer/9008080#meta_tag_verification&zippy=%2Chtml-tag) dans AstroPaper en utilisant une variable d'environment. Cette étape est optionnelle. Si vous n'ajoutez pas la variable, Le tag google-site-verification n'appraitra pas dans l'entête html `<head>` section.

```bash
# in your environment variable file (.env)
PUBLIC_GOOGLE_SITE_VERIFICATION=your-google-site-verification-value
```

## 🧞 Commands

Toutes les commandes sont exécutées depuis la racine du projet, à partir d'un terminal:

> **_Note!_** Pour les commandes `Docker` nous devons avoir [installé](https://docs.docker.com/engine/install/) sur la machine.

| Command                              | Action                                                                                                                           |
| :----------------------------------- | :------------------------------------------------------------------------------------------------------------------------------- |
| `npm install`                        | Installs dependencies                                                                                                            |
| `npm run dev`                        | Starts local dev server at `localhost:4321`                                                                                      |
| `npm run build`                      | Build your production site to `./dist/`                                                                                          |
| `npm run preview`                    | Preview your build locally, before deploying                                                                                     |
| `npm run format:check`               | Check code format with Prettier                                                                                                  |
| `npm run format`                     | Format codes with Prettier                                                                                                       |
| `npm run sync`                       | Generates TypeScript types for all Astro modules. [Learn more](https://docs.astro.build/en/reference/cli-reference/#astro-sync). |
| `npm run cz`                         | Commit code changes with commitizen                                                                                              |
| `npm run lint`                       | Lint with ESLint                                                                                                                 |
| `docker compose up -d`               | Run AstroPaper on docker, You can access with the same hostname and port informed on `dev` command.                              |
| `docker compose run app npm install` | You can run any command above into the docker container.                                                                         |

> **_Warning!_** Les utilisateurs Windows PowerShell devront installer la [paquet concurrently](https://www.npmjs.com/package/concurrently) s'ils souhaitent [exécuter les diagnostiques](https://docs.astro.build/en/reference/cli-reference/#astro-check) durant le dévelopment (`astro check --watch & astro dev`). Pour plus d'info, voir [cette référence](https://github.com/satnaing/astro-paper/issues/113).

## ✨ Feedback & Suggestions

Si vous avez des suggestions/feedback, vous pouvez contacter [Satnaing](mailto:contact@satnaing.dev). Sentez vous libre d'ouvrir un ticket si vous identifiez des bugs ou vous voulez demander une nouvelle fonctionnalité.

## 📜 License

Licensed under the MIT License, Copyright © 2023

---

Crée par 🤍 by [Sat Naing](https://satnaing.dev) 👨🏻‍💻 & [contributors](https://github.com/satnaing/astro-paper/graphs/contributors).
Traduit par [Amaury](https://amauryvanespen.github.io/)
