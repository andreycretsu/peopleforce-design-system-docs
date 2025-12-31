# People Force Design System - Component Documentation

Welcome to the comprehensive component documentation for the People Force Design System. This repository contains detailed guides, code examples, and design specifications for all UI components.

## 📚 Component Index

### Base Components

#### 1. **Avatar**
User profile images or initials display component
- **Status**: Ready
- - **Package**: @peopleforce/ui
  - - **Documentation**: [Avatar Component](./avatar/README.md)
    -   - [Vue.js Implementation](./avatar/vue.md)
        -   - [Rails Implementation](./avatar/rails.md)
            -   - [Figma Design](./avatar/figma.md)
             
                - #### 2. **AvatarStack** *(Coming Soon)*
                - Groups of avatars with overflow handling
                - - Display multiple user avatars in a compact space
                  - - Customize stacking behavior and sizing
                   
                    - #### 3. **Badge** *(Coming Soon)*
                    - Status and count indicators
                    - - Multiple variants (success, warning, danger, info)
                      - - Size options (small, medium, large)
                       
                        - #### 4. **BottomSheet** *(Coming Soon)*
                        - Mobile-friendly modal component
                        - - Swipe-dismissible interface
                          - - Customizable height and animations
                           
                            - #### 5. **Button** *(Coming Soon)*
                            - Primary action element
                            - - Multiple variants (primary, secondary, danger, ghost)
                              - - Size options and loading states
                               
                                - #### 6. **ButtonGroup** *(Coming Soon)*
                                - Multiple buttons grouped together
                                - - Vertical and horizontal layouts
                                  - - Connected button styling
                                   
                                    - #### 7. **EmployeeHoverCard** *(Coming Soon)*
                                    - User information preview on hover
                                    - - Quick user details display
                                      - - Customizable content and actions
                                       
                                        - #### 8. **FieldIcon** *(Coming Soon)*
                                        - Icon placement in form fields
                                        - - Leading and trailing icon support
                                          - - Interactive icon functionality
                                           
                                            - ---

                                            ## 🎯 Documentation Structure

                                            Each component includes:

                                            - **Overview**: General description, anatomy, usage guidelines
                                            - - **Vue.js Implementation**: Code examples with Storybook link
                                              - - **Rails Implementation**: ViewComponent examples with Lookbook link
                                                - - **Figma Design**: Visual specifications and design tokens
                                                 
                                                  - ---

                                                  ## 🚀 Getting Started

                                                  ### For Developers

                                                  1. **Vue.js/JavaScript**: See the Vue.js implementation section in each component
                                                  2.    ```bash
                                                           npm install @peopleforce/ui
                                                           ```

                                                        2. **Rails**: Use ViewComponent from the Rails implementation section
                                                        3.    ```ruby
                                                                 bundle add primer_view_components
                                                                 ```

                                                              3. **Examples**: Each component includes copy-paste ready code examples
                                                          
                                                              4. ### For Designers
                                                          
                                                              5. 1. Access Figma files for each component (links in Figma Design section)
                                                                 2. 2. Review size systems, colors, and spacing guidelines
                                                                    3. 3. Export assets and specifications as needed
                                                                      
                                                                       4. ---
                                                                      
                                                                       5. ## 📋 Documentation Format
                                                                      
                                                                       6. ### Overview Tab
                                                                       7. - General description and use cases
                                                                          - - Component anatomy (visual breakdown)
                                                                            - - When to use / When NOT to use
                                                                              - - Best practices and guidelines
                                                                                - - Properties table
                                                                                  - - Variations
                                                                                   
                                                                                    - ### View JS Tab
                                                                                    - - JavaScript/Vue.js import statements
                                                                                      - - 5+ practical code examples
                                                                                        - - Link to interactive Storybook
                                                                                          - - Props and slots reference
                                                                                            - - Event handling examples
                                                                                             
                                                                                              - ### Rails Tab
                                                                                              - - Rails ViewComponent syntax
                                                                                                - - ERB template examples
                                                                                                  - - Integration with Rails views
                                                                                                    - - Link to Lookbook preview
                                                                                                      - - Helper methods and options
                                                                                                       
                                                                                                        - ### Figma Tab
                                                                                                        - - Design specifications
                                                                                                          - - Size system and spacing
                                                                                                            - - Color palette and typography
                                                                                                              - - Interactive Figma file embed
                                                                                                                - - Design tokens
                                                                                                                 
                                                                                                                  - ---
                                                                                                                  
                                                                                                                  ## 🔗 Quick Links
                                                                                                                  
                                                                                                                  - [Storybook](https://storybook.stage-81y92gtmor-peopleforce.dev) - Interactive component preview
                                                                                                                  - - [Figma Design Files](https://figma.com) - Design specifications
                                                                                                                    - - [Package Repository](https://npmjs.com/@peopleforce/ui) - NPM package
                                                                                                                     
                                                                                                                      - ---
                                                                                                                      
                                                                                                                      ## 🛠️ Contributing
                                                                                                                      
                                                                                                                      ### Adding New Component Documentation
                                                                                                                      
                                                                                                                      1. Create a new folder under `docs/components/{component-name}/`
                                                                                                                      2. 2. Create `README.md` with overview content
                                                                                                                         3. 3. Add `vue.md` with Vue.js implementation examples
                                                                                                                            4. 4. Add `rails.md` with Rails ViewComponent examples
                                                                                                                               5. 5. Add `figma.md` with design specifications
                                                                                                                                  6. 6. Update this INDEX.md file with the new component
                                                                                                                                    
                                                                                                                                     7. ### Template
                                                                                                                                    
                                                                                                                                     8. See [Component Template](./TEMPLATE.md) for the standard structure to follow when documenting new components.
                                                                                                                                    
                                                                                                                                     9. ---
                                                                                                                                    
                                                                                                                                     10. ## 📞 Questions or Feedback?
                                                                                                                                    
                                                                                                                                     11. For documentation improvements or questions about components:
                                                                                                                                     12. - Open an Issue in the repository
                                                                                                                                         - - Check existing component documentation
                                                                                                                                           - - Review code examples in Storybook
                                                                                                                                            
                                                                                                                                             - ---
                                                                                                                                             
                                                                                                                                             ## 📅 Last Updated
                                                                                                                                             
                                                                                                                                             December 31, 2025
                                                                                                                                             
                                                                                                                                             **Version**: 1.0.0
                                                                                                                                             **Status**: In Progress (Avatar component completed, others in development)
