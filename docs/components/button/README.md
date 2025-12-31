# Button Component

## Overview

The Button component is the primary interactive element used to trigger actions or navigation. It's a fundamental building block for all interactive experiences in the application.

**Status**: Ready | **Package**: @peopleforce/ui

## Quick Links

- [Vue.js Implementation](./vue.md)
- - [Rails Implementation](./rails.md)
  - - [Figma Design](./figma.md)
   
    - ---

    ## Anatomy

    - **Label**: Text content indicating button action
    - - **Icon (optional)**: Visual indicator before/after text
      - - **Focus State**: Clear visual focus indicator
        - - **Loading State**: Spinner indicator for async actions
          - - **Disabled State**: Visual indication of disabled state
           
            - ---

            ## Usage

            ### When to Use ✓

            - Primary actions (submit, save, create)
            - - Secondary actions (cancel, back, close)
              - - Navigation triggers
                - - Form submissions
                  - - Confirmation actions
                   
                    - ### When NOT to Use ✗
                   
                    - - Text-only navigation (use Link instead)
                      - - Inline text actions (use inline button)
                        - - Disabled permanently (remove rather than disable)
                         
                          - ---

                          ## Best Practices

                          ### Do's ✓

                          - Use clear, actionable labels
                          - - Provide proper spacing around buttons
                            - - Show loading state for async operations
                              - - Ensure sufficient contrast
                                - - Use consistent sizing within sections
                                 
                                  - ### Don'ts ✗
                                 
                                  - - Don't use vague labels ("Click here")
                                    - - Don't disable buttons unnecessarily
                                      - - Don't use too many primary buttons
                                        - - Don't nest buttons
                                          - - Don't use buttons for navigation only
                                           
                                            - ---

                                            ## Properties

                                            | Property | Type | Default | Description |
                                            |----------|------|---------|-------------|
                                            | `variant` | "primary" \| "secondary" \| "danger" \| "ghost" | "primary" | Button style |
                                            | `size` | "small" \| "medium" \| "large" | "medium" | Button size |
                                            | `disabled` | boolean | false | Disabled state |
                                            | `loading` | boolean | false | Loading state |
                                            | `icon` | string | - | Icon name |
                                            | `fullWidth` | boolean | false | Full width button |

                                            ---

                                            ## Variants

                                            - **Primary**: Main action button (blue)
                                            - - **Secondary**: Alternative action (gray)
                                              - - **Danger**: Destructive actions (red)
                                                - - **Ghost**: Minimal style (transparent)
                                                 
                                                  - ---

                                                  ## States

                                                  - **Default**: Normal button state
                                                  - - **Hover**: Interactive feedback
                                                    - - **Active**: Pressed state
                                                      - - **Disabled**: Non-interactive
                                                        - - **Loading**: Async operation in progress
                                                          - - **Focus**: Keyboard navigation
                                                           
                                                            - ---

                                                            ## Related Components

                                                            - [ButtonGroup](../button-group/README.md) - Multiple grouped buttons
                                                            - - [Badge](../badge/README.md) - Status indicators
                                                              - - [Link](#) - Text navigation
