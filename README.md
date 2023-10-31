# JMX2 template notes

This is a repo that is used to make experimental layouts. It uses Astro to build the site. It is a fork of the Astro starter kit.


## GSAP instructions

This installation assume you have GSAP Business, https://gsap.com/pricing/, which requires a token from GSAP.com. See: https://gsap.com/docs/v3/Installation/ about setting up your token and creating a `.npmrc` file. The reason for this is that the GSAP Club plugins are not available on NPM.

GSAP is shown in the `package.json` file has this line:

```json
"gsap": "gsap@npm:@greensock/gsap-business"
```

If you don't need the extra GSAP Club plugins, you can use the free version of GSAP. See: https://greensock.com/docs/v3/Installation

You can remove that line from the `package.json` file and replace it with this line:

```json
"gsap": "gsap"
```

## Finishing Set up

Now that you've got GSAP sorted, you can run the following commands to get the site up and running.


## To run

```sh
npm install
```

```sh
npm run dev
```

## To build for deployment

```sh
npm run build
```

You will now have a `dist` folder that you can deploy to a static site host.



## Below are the original Astro starter kit notes.



# Astro Starter Kit: Basics

```sh
npm create astro@latest -- --template basics
```

[![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/withastro/astro/tree/latest/examples/basics)
[![Open with CodeSandbox](https://assets.codesandbox.io/github/button-edit-lime.svg)](https://codesandbox.io/p/sandbox/github/withastro/astro/tree/latest/examples/basics)
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/withastro/astro?devcontainer_path=.devcontainer/basics/devcontainer.json)

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

![just-the-basics](https://github.com/withastro/astro/assets/2244813/a0a5533c-a856-4198-8470-2d67b1d7c554)

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   └── Card.astro
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
