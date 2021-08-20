A common Prettier config used in AQS's projects.

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

2. Install Prettier and this package.

   ```bash
   yarn add --dev prettier @aq-systems/prettier-config
   ```

3. Add the follow config file (`/prettier.config.js`) at the root of your project.

   ```js
   // prettier.config.js
   module.exports = require('@swingby-protocol/prettier-config');
   ```
