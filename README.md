# Vue 2 + TypeScript + Vite + Vuetify

<p align="center">
  <img src="https://user-images.githubusercontent.com/480173/157433906-7f7910d4-6430-49f4-857a-044945e71360.png" alt="logo" width="300" height="300" />
</p>

This is a [starter project](https://github.com/logue/vite-vue2-ts-starter) that uses [Vuetify](https://vuetifyjs.com/) as the UI framework. Please use scss version 1.32.12 due to a problem on the Vuetify side.

Vuetify3 version is [here](https://github.com/logue/vite-vuetify-ts-starter).

## Description

This template is for using Vue2 with TypeScript in Vite. Includes [vue-router](https://router.vuejs.org/) and [Vuex](https://vuex.vuejs.org/), [vue-property-decorator](https://github.com/kaorun343/vue-property-decorator).

In addition, [ESLint](https://eslint.org/), [Stylelint](https://stylelint.io/), and [Prettier](https://prettier.io/) are also included and are set to be executed automatically at runtime and commit. (Since these settings are set strictly, please relax yourself.)

## Recommended IDE Setup

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=johnsoncodehk.volar) (and disable Vetur).

## Commands

| Command     | Description                                        |
| ----------- | -------------------------------------------------- |
| dev         | Start devserver.                                   |
| clean       | Clear devserver cache.                             |
| build       | Build for production                               |
| build:clean | Clear production build files.                      |
| lint        | Run ESLint and prettier.                           |
| lint:style  | Run Stylelint.                                     |
| lint:markup | Check vue markup.                                  |
| preview     | Run the program generated by the production build. |

## Migrate from VueCli

It also works when migrating from VueCLI.

However, when importing a stylesheet with `@import`, it cannot be specified from the library directory. Must be specified from `~node_modules/`.

Also, if you used the .env file in the previous environment, you need to change the calling part from `process.env` to `import.meta.env` after installing [vite-plugin-env-compatible](https://github.com/IndexXuan/vite-plugin-env-compatible) separately.

## Troubleshooting

When adding or deleting files, an error may occur and even if the error is corrected, it may not be reflected in devserver. In that case, stop devserver and delete all the files in the `node_modules/.vite` directory. You can also run it with the `clean` command.
