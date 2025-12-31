# AvatarStack Component

## Overview

The AvatarStack component is used to display multiple user avatars in a compact, stackable manner. It efficiently shows groups of people with overflow handling and tooltips for additional users.

**Status**: Ready | **Package**: @peopleforce/ui

## Quick Links

- [Vue.js Implementation](./vue.md)
- - [Rails Implementation](./rails.md)
  - - [Figma Design](./figma.md)
   
    - ---

    ## Anatomy

    - **Avatar Container**: The stacked visual layout
    - - **Individual Avatars**: User profile images in the stack
      - - **Overflow Indicator**: Shows count of hidden users (+N)
        - - **Tooltip**: Displays names of all users on hover
          - - **Spacing**: Controlled overlap between avatars
           
            - ---

            ## Usage

            ### When to Use ✓

            - Displaying team members or collaborators
            - - Showing participant lists with limited space
              - - Viewing activity by multiple users
                - - Indicating group assignment
                 
                  - ### When NOT to Use ✗
                 
                  - - Showing single user (use Avatar instead)
                    - - Displaying non-user entities
                      - - When individual users need prominence
                       
                        - ---

                        ## Best Practices

                        ### Do's ✓

                        - Use consistent avatar sizes
                        - - Limit visible avatars (3-5 recommended)
                          - - Show overflow count clearly
                            - - Provide tooltips with full names
                              - - Order by relevance or alphabetically
                               
                                - ### Don'ts ✗
                               
                                - - Don't show more than 7-8 avatars without hiding
                                  - - Don't remove overflow indicators
                                    - - Don't use irregular image sizes
                                      - - Don't mix with other components in same line
                                       
                                        - ---

                                        ## Properties

                                        | Property | Type | Default | Description |
                                        |----------|------|---------|-------------|
                                        | `avatars` | Avatar[] | - | List of avatars to display |
                                        | `max` | number | 5 | Maximum visible avatars |
                                        | `size` | number | 32 | Avatar size in pixels |
                                        | `direction` | "ltr" \| "rtl" | "ltr" | Stack direction |

                                        ---

                                        ## Variations

                                        - **Default**: Standard stacked avatars
                                        - - **Open**: Expanded view showing all avatars
                                          - - **Custom Tooltip**: Custom hover information
                                            - - **Palette**: Multiple size variations
                                              - - **Overflow**: Shows +N indicator
                                               
                                                - ---

                                                ## Related Components

                                                - [Avatar](../avatar/README.md) - Individual user avatar
                                                - - [Badge](../badge/README.md) - Status indicators
                                                  - - [EmployeeHoverCard](../employee-hover-card/README.md) - User info preview
