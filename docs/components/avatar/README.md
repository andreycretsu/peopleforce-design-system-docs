# Avatar Component

## Overview

The Avatar component is used to display a user's profile image or initials. It's a fundamental UI element for representing individuals in various contexts such as user profiles, comments, team members, and authentication states.

**Status**: Ready | **Package**: @peopleforce/ui

## Quick Links

- [Vue.js Implementation](./vue.md)
- - [Rails Implementation](./rails.md)
  - - [Figma Design](./figma.md)
   
    - ---

    ## Anatomy

    The Avatar component consists of:

    - **Image Container**: The circular or rounded container holding the visual content
    - - **Image**: The user's profile photo
      - - **Fallback**: Initials displayed when no image is available
        - - **Status Badge (optional)**: Indicator for online/offline status
          - - **Border (optional)**: Border for emphasis or visual separation
           
            - ---

            ## Usage

            ### When to Use ✓

            - Displaying user profiles or team members
            - - Showing comment authors or activity participants
              - - Indicating the current logged-in user
                - - Representing people in lists or tables
                 
                  - ### When Not to Use ✗
                 
                  - - Non-human entities (use icons instead)
                    - - Displaying large product images
                      - - Company logos in lists (use alternative component)
                       
                        - ---

                        ## Best Practices

                        ### Do's ✓

                        - Use consistent sizing within containers
                        - - Always provide fallback initials
                          - - Use appropriate sizing for context (12-20px compact, 32px default, 48px+ prominent)
                            - - Pair with status indicators when relevant
                              - - Ensure square, properly cropped images
                               
                                - ### Don'ts ✗
                               
                                - - Don't use irregular or non-square images
                                  - - Don't mix sizes randomly without hierarchy
                                    - - Don't rely only on images without text fallback
                                      - - Don't use for non-human representations
                                       
                                        - ---

                                        ## Properties

                                        | Property | Type | Default | Description |
                                        |----------|------|---------|-------------|
                                        | `size` | 12 \| 16 \| 20 \| 24 \| 32 \| 36 \| 40 \| 48 | 32 | Avatar size in pixels |
                                        | `url` | string \| null | null | Image URL |
                                        | `text` | string | - | Person name for initials |
                                        | `border` | boolean | false | Show border |
                                        | `checked` | boolean | undefined | Selection state |
                                        | `status` | "green" \| "yellow" \| "red" \| null | null | Status indicator |

                                        ---

                                        ## Size System

                                        - **Extra Small** (12px): Compact UI spaces, nested components
                                        - - **Small** (16-20px): List items, comments, notifications
                                          - - **Medium** (32px): Default size for most use cases
                                            - - **Large** (40-48px): Profile pages, card headers
                                              - - **Extra Large** (64px+): Hero sections, detail views
                                               
                                                - ---

                                                ## Examples

                                                ### Basic Avatar

                                                ```vue
                                                <PfAvatar
                                                  text="John Doe"
                                                  url="/img/avatar.png"
                                                  size="32"
                                                />
                                                ```

                                                ### With Status

                                                ```vue
                                                <PfAvatar
                                                  text="Jane Smith"
                                                  url="/img/jane.png"
                                                  size="40"
                                                  status="green"
                                                />
                                                ```

                                                ### With Border

                                                ```vue
                                                <PfAvatar
                                                  text="John Doe"
                                                  url="/img/avatar.png"
                                                  size="40"
                                                  :border="true"
                                                />
                                                ```

                                                ### Fallback (No Image)

                                                ```vue
                                                <PfAvatar
                                                  text="John Doe"
                                                  size="32"
                                                />
                                                <!-- Displays initials when URL is not provided -->
                                                ```

                                                ---

                                                ## Variations

                                                - **Default**: Standard avatar with image and fallback
                                                - - **Status**: Avatar with status indicator
                                                  - - **Palette**: Multiple avatar sizes
                                                    - - **Fallback**: Initials mode
                                                      - - **Border**: With border emphasis
                                                        - - **Checkbox**: Interactive selection
                                                         
                                                          - ---

                                                          ## Accessibility

                                                          - Always provide text description (name or initials)
                                                          - - Ensure sufficient contrast for initials
                                                            - - Use semantic HTML for interactive variants
                                                              - - Include aria-labels when needed for screen readers
                                                               
                                                                - ---

                                                                ## Related Components

                                                                - [AvatarStack](../avatar-stack/README.md) - Groups of avatars
                                                                - - [Badge](../badge/README.md) - Status indicators
                                                                  - - [EmployeeHoverCard](../employee-hover-card/README.md) - User info preview
