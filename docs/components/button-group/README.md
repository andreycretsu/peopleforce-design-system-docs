# ButtonGroup Component

## Overview

The ButtonGroup component groups multiple buttons together for related actions. It provides clear visual and functional grouping while maintaining individual button functionality.

**Status**: Ready | **Package**: @peopleforce/ui

## Quick Links

- [Vue.js Implementation](./vue.md)
- - [Rails Implementation](./rails.md)
  - - [Figma Design](./figma.md)
   
    - ---

    ## Anatomy

    - **Container**: The grouping wrapper
    - - **Buttons**: Individual button elements
      - - **Dividers**: Separators between buttons (optional)
        - - **Selected State**: Highlight active button (toggle groups)
         
          - ---

          ## Usage

          ### When to Use ✓

          - Segmented controls (view options)
          - - Related actions grouped together
            - - Toggle button groups
              - - Filter/sort options
               
                - ### When NOT to Use ✗
               
                - - Unrelated actions (use Button separately)
                  - - Too many buttons (5+ use select/dropdown instead)
                    - - Single buttons (use Button component)
                     
                      - ---

                      ## Properties

                      | Property | Type | Default | Description |
                      |----------|------|---------|-------------|
                      | `orientation` | "horizontal" \| "vertical" | "horizontal" | Button layout |
                      | `variant` | "filled" \| "outlined" | "filled" | Button style |
                      | `size` | "small" \| "medium" \| "large" | "medium" | Button size |
                      | `connected` | boolean | true | Connected/separated buttons |

                      ---

                      ## Layouts

                      - **Horizontal**: Side-by-side arrangement
                      - - **Vertical**: Stacked arrangement
                        - - **Connected**: Buttons touching with shared borders
                          - - **Separated**: Buttons with gaps between
                           
                            - ---

                            ## Related Components

                            - [Button](../button/README.md) - Individual button
                            - - [Segmented Control](#) - Similar for selections
