# Badge Component

## Overview

The Badge component is a visual indicator used to display status, count, or classification information in a compact, inline format. It's commonly used for notifications, status indicators, and tagging information.

**Status**: Ready | **Package**: @peopleforce/ui

## Quick Links

- [Vue.js Implementation](./vue.md)
- - [Rails Implementation](./rails.md)
  - - [Figma Design](./figma.md)
   
    - ---

    ## Anatomy

    - **Container**: The badge background shape
    - - **Label**: Text content indicating status or count
      - - **Icon (optional)**: Visual indicator before or after text
        - - **Color**: Semantic color indicating type (success, warning, danger, info)
         
          - ---

          ## Usage

          ### When to Use ✓

          - Displaying status (active, inactive, pending)
          - - Showing notification counts
            - - Indicating labels or categories
              - - Highlighting new or important information
                - - Showing availability or presence
                 
                  - ### When NOT to Use ✗
                 
                  - - Large amounts of descriptive text
                    - - Primary interactive actions (use Button instead)
                      - - Complex data that needs tables
                       
                        - ---

                        ## Best Practices

                        ### Do's ✓

                        - Use semantic colors (green=success, red=danger, yellow=warning)
                        - - Keep text short and concise
                          - - Use appropriate size for context
                            - - Combine with icons when helpful
                              - - Use consistent styling within sections
                               
                                - ### Don'ts ✗
                               
                                - - Don't use too many different badge types on one page
                                  - - Don't make badges interactive (static status only)
                                    - - Don't use too many colors
                                      - - Don't add unnecessary icons
                                       
                                        - ---

                                        ## Properties

                                        | Property | Type | Default | Description |
                                        |----------|------|---------|-------------|
                                        | `variant` | "default" \| "success" \| "warning" \| "danger" \| "info" | "default" | Badge type |
                                        | `size` | "small" \| "medium" \| "large" | "medium" | Badge size |
                                        | `text` | string | - | Badge label text |
                                        | `count` | number | - | Numeric value to display |
                                        | `icon` | string | - | Icon name to display |

                                        ---

                                        ## Variants

                                        - **Default**: Neutral badge for general information
                                        - - **Success**: Green badge for positive status
                                          - - **Warning**: Yellow badge for caution/warning
                                            - - **Danger**: Red badge for error/critical status
                                              - - **Info**: Blue badge for informational content
                                               
                                                - ---

                                                ## Sizes

                                                - **Small**: 16px height (tight contexts)
                                                - - **Medium**: 24px height (default)
                                                  - - **Large**: 32px height (prominent display)
                                                   
                                                    - ---

                                                    ## Examples

                                                    ### Status Badge
                                                    ```vue
                                                    <PfBadge variant="success" text="Active" />
                                                    <PfBadge variant="warning" text="Pending" />
                                                    <PfBadge variant="danger" text="Error" />
                                                    ```

                                                    ### Count Badge
                                                    ```vue
                                                    <PfBadge :count="5" />
                                                    <PfBadge :count="99+" />
                                                    ```

                                                    ### With Icon
                                                    ```vue
                                                    <PfBadge variant="success" icon="check" text="Verified" />
                                                    ```

                                                    ---

                                                    ## Related Components

                                                    - [Avatar](../avatar/README.md) - User profile display
                                                    - - [Button](../button/README.md) - Interactive actions
                                                      - - [Tag (coming soon)](#) - Similar for multiple selections
