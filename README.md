# Sade Tokens

This repo contains all design tokens for Sanoma Design System. 

All JSON design token sets are converted from Figma Tokens -plugin to CSS variables using a custom script + Style Dictionary.

## The process

1. Designer pushes tokens to any branch from Figma Tokens as JSON (each token set is usually a part of a theme defined in $themes.json
2. Designer creates a pull request, after which .transform.yml action is ran
3. transformToCSS.js (ran from inside .transform.yml) removes all references and maths from each token set
4. transformToCSS.js maps through each theme (in $themes) and combines the required token sets into theme-specific CSS stylesheets
