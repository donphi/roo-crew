# Configuration-Driven Architecture Enforcement

You MUST ensure that every agent strictly adheres to the centralized configuration principle. Design specific mechanisms for configuration validation, automated auditing of code for hardcoded values, and systematic enforcement of the "single source of truth" paradigm across all visual and functional components, regardless of the specific technology stack selected.

## Key Implementation Points:

1. **Centralized Configuration System**: Establish a robust, hierarchical configuration system that serves as the single source of truth for all styling, theming, and configurable parameters across the selected **Frontend Framework**, **Styling Framework**, and **Data Visualization** components.

2. **Automated Compliance Verification**: Implement automated checks using the selected **Code Quality Tools** that scan code for hardcoded values or direct style manipulations that bypass the central configuration system.

3. **Configuration Inheritance Patterns**: Design clear patterns for how configuration values cascade and override each other, with explicit documentation of the precedence rules appropriate for the selected technology stack.

4. **Runtime Configuration Validation**: Create mechanisms to validate configuration integrity at runtime, ensuring that all components are correctly sourcing their properties from the central system, leveraging the selected **Testing Frameworks** for validation.

5. **Configuration Change Impact Analysis**: Develop tools to predict and visualize the impact of configuration changes across the entire application before they are applied, integrated with the selected **CI/CD Pipeline**.

This architecture ensures that the application's look and feel can be modified comprehensively by changing only the central configuration files, dramatically reducing maintenance overhead and ensuring visual consistency throughout the application lifecycle, regardless of which specific technologies are selected from the TECHNOLOGY ARSENAL.