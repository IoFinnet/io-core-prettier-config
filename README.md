A common Prettier config used in Iofinnets's projects.

## Quick start

1. Add the following EditorConfig config file (`/.editorconfig`) at the root of your project.

   ```editorconfig
   # .editorconfig

   root = true

   [*]
   indent_style = space
   indent_size = 2
   end_of_line = lf
   charset = utf-8
   trim_trailing_whitespace = true
   insert_final_newline = true

   [*.md]
   trim_trailing_whitespace = false
   ```

2. Install Prettier and this package (see
   [Downloading private `@iofinnet` packages](#downloading-private-iofinnet-packages)).

   ```bash
   yarn add --dev prettier @iofinnet/io-core-fedev-prettier-config
   ```

3. Add the follow config file (`/prettier.config.js`) at the root of your project.

   ```js
   // prettier.config.js
   module.exports = require('@iofinnet/io-core-fedev-prettier-config');
   ```

### Downloading private `@iofinnet` packages

1. Make sure your repo contains an `.npmrc` file at its root with the following content.

   ```.npmrc
   @iofinnet:registry=https://npm.pkg.github.com
   ```

2. Run the following command once.

   ```bash
   npm login --scope=@iofinnet --registry=https://npm.pkg.github.com
   ```

   When prompted for a password, paste a [Personal access token](https://github.com/settings/tokens)
   for your GitHub account that has the scope `read:packages`.
