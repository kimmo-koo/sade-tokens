# Sade Tokens

This repo demostrates converting design tokens from Figma Tokens -plugin to CSS variables using a custom script + Style Dictionary.

## The process

1. Tokens are pushed to a branch from Figma Tokens as JSON (each token set is usually a part of a theme defined in $themes.json
2. transformToCSS.js removes all references and maths from each token set
3. transformToCSS.js maps through each theme and combines the required token sets into single CSS stylesheets (one per theme).

