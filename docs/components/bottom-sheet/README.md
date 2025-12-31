# BottomSheet Component

## Overview

The BottomSheet component is a mobile-friendly modal that slides up from the bottom of the screen. It's ideal for presenting content that doesn't require full-screen attention and supports dismissal via swipe or click-outside.

**Status**: Ready | **Package**: @peopleforce/ui

## Quick Links

- [Vue.js Implementation](./vue.md)
- - [Rails Implementation](./rails.md)
  - - [Figma Design](./figma.md)
   
    - ---

    ## Anatomy

    - **Backdrop**: Semi-transparent overlay behind the sheet
    - - **Handle**: Visual indicator for dragging (optional)
      - - **Header**: Title and close button area
        - - **Content**: Main scrollable content area
          - - **Footer**: Fixed action buttons (optional)
            - - **Rounded Corners**: Top corners only
             
              - ---

              ## Usage

              ### When to Use ✓

              - Mobile forms and input dialogs
              - - Action menus on mobile
                - - Viewing detailed information
                  - - Settings or preferences on mobile
                    - - Share sheets and similar patterns
                     
                      - ### When NOT to Use ✗
                     
                      - - Desktop-first experiences (use Modal instead)
                        - - Critical information requiring full focus
                          - - Very long content (consider full page)
                           
                            - ---

                            ## Best Practices

                            ### Do's ✓

                            - Keep content focused and concise
                            - - Provide clear close/confirm actions
                              - - Support both drag and click-to-dismiss
                                - - Use appropriate height (30-80% of screen)
                                  - - Make actions clear and prominent
                                   
                                    - ### Don'ts ✗
                                   
                                    - - Don't nest BottomSheets
                                      - - Don't force maximum height
                                        - - Don't hide dismiss options
                                          - - Don't use for critical operations without confirmation
                                           
                                            - ---

                                            ## Properties

                                            | Property | Type | Default | Description |
                                            |----------|------|---------|-------------|
                                            | `open` | boolean | false | Whether sheet is visible |
                                            | `title` | string | - | Header title text |
                                            | `height` | "small" \| "medium" \| "large" | "medium" | Sheet height |
                                            | `dismissible` | boolean | true | Allow dismiss on backdrop click |
                                            | `draggable` | boolean | true | Show and allow drag handle |

                                            ---

                                            ## Behavior

                                            - **Swipe Up**: Expand (if small/medium)
                                            - - **Swipe Down**: Dismiss (if not locked)
                                              - - **Click Backdrop**: Dismiss (if dismissible=true)
                                                - - **Scroll Content**: While sheet is open
                                                 
                                                  - ---

                                                  ## Related Components

                                                  - [Modal](../modal/README.md) - Full-screen modal
                                                  - - [Dialog](#) - Desktop dialog equivalent
                                                    - - [Drawer](#) - Side panel alternative
