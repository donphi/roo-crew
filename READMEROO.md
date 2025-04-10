# 🧠 Visionary Recruiter Template

## Overview

This template provides a comprehensive framework for creating and managing a team of specialized AI agents for robust production-grade web applications. It uses the Roo Code custom modes feature to create a "Visionary Recruiter" that can design and recruit specialized agent teams tailored to your project's specific needs.

## 🗂️ Template Structure

```
.
├── .env.example                      # Environment variables template
├── .gitignore                        # Comprehensive Git exclusion rules
├── .recruitment_prompt               # Main prompt for the Visionary Recruiter
├── .roo/                             # Roo configuration directory
│   ├── modes/                        # Custom mode definitions
│   │   └── visionary-recruiter.json  # Visionary Recruiter mode definition
│   ├── rules/                        # Global rules for all agents
│   │   ├── 01_code_quality_standards.md
│   │   ├── 02_security_protocols.md
│   │   └── 03_deployment_readiness.md
│   └── rules-visionary-recruiter/    # Rules specific to the Visionary Recruiter
│       ├── 01_future_oriented_agent_ecosystem.md
│       ├── 02_modular_team_structure.md
│       ├── 03_predictive_error_management.md
│       ├── 04_configuration_driven_architecture.md
│       ├── 05_documentation_as_living_system.md
│       └── 06_agent_communication_protocol.md
└── .roomodes                         # Project-specific mode registration
```

## 🚀 Getting Started

### 1. Setup

1. Clone this template repository
2. Copy `.env.example` to `.env` and update the values as needed
3. Ensure the Visionary Recruiter mode is properly registered:
   - The `.roomodes` file should contain the proper JSON configuration
   - The `.roo/modes/visionary-recruiter.json` file should be present
   - The `.roo/rules-visionary-recruiter/` directory should contain the rule files

### 2. Using the Visionary Recruiter

1. Switch to the "🧠 Visionary Recruiter" mode in Roo Code
2. Provide the `.recruitment_prompt` content to the Visionary Recruiter
3. The Visionary Recruiter will analyze your requirements and design a specialized team of AI agents

## 📝 Customization Guide

### Modifying the Tech Stack

The default template is configured for a TypeScript/Next.js/Tailwind/Supabase/ECharts stack. To adapt it to your specific tech stack:

1. Edit the `.recruitment_prompt` file:
   - Modify the "Technology Stack" section to list your specific technologies
   - Update the "Architectural Principles" section to reflect your project's architecture
   - Adjust the "Development Process" section if your workflow differs

```markdown
**Technology Stack:**
*   Frontend: [Your frontend framework]
*   Language: [Your programming language]
*   Styling: [Your styling solution]
*   UI Components: [Your component library]
*   Data Visualization: [Your visualization library]
*   Backend/DB: [Your backend/database solution]
```

### Adding Custom Rules

1. Global Rules (apply to all agents):
   - Add new rule files to `.roo/rules/` directory
   - Follow the naming convention: `XX_rule_name.md`

2. Visionary Recruiter Rules:
   - Add new rule files to `.roo/rules-visionary-recruiter/` directory
   - Follow the naming convention: `XX_rule_name.md`

3. Agent-Specific Rules:
   - For each agent created by the Visionary Recruiter, create a directory:
     `.roo/rules-{agent-slug}/`
   - Add rule files following the naming convention: `XX_rule_name.md`

### Modifying the Visionary Recruiter

If you need to adjust the Visionary Recruiter's capabilities:

1. Edit `.roo/modes/visionary-recruiter.json`:
   - Modify the `roleDefinition` to change the recruiter's expertise
   - Adjust the `groups` to change the recruiter's permissions
   - Update the `customInstructions` to change the recruiter's behavior

2. Update `.roomodes` to reflect any changes to the mode configuration

## 🛠️ Advanced Configuration

### Environment Variables

The `.env.example` file provides a comprehensive template for environment variables. Customize it to include:

- API keys and secrets
- Database connection strings
- Feature flags
- Environment-specific configuration

### Git Configuration

The `.gitignore` file is configured to exclude:

- Environment files (.env)
- Dependency directories (node_modules)
- Build artifacts
- IDE files
- Operating system files
- Logs and debugging files

Modify it as needed for your specific project requirements.

## 📋 Running the Recruitment Process

1. Switch to the "🧠 Visionary Recruiter" mode in Roo Code
2. Provide a prompt like:

```
I need to build a [your project description]. Please analyze the requirements and design a team of specialized AI agents to build, maintain, and manage this application.
```

3. The Visionary Recruiter will:
   - Analyze your requirements
   - Design a team of specialized agents
   - Define each agent's role, responsibilities, and permissions
   - Create JSON definitions for each agent
   - Provide instructions for implementing the agent team

4. Implement the suggested agent team:
   - Create the agent JSON definitions in `.roo/modes/`
   - Update `.roomodes` to register the agents
   - Create rule files for each agent in `.roo/rules-{agent-slug}/`

5. Use the specialized agents to build your application:
   - Switch between agents as needed for different tasks
   - Each agent will have specific expertise and permissions
   - The agents will collaborate to build a robust, production-grade application

## 🔄 Workflow Example

1. **Visionary Recruiter**: Design the agent team
2. **Project Orchestrator**: Coordinate the overall workflow
3. **UI Theme Manager**: Define the centralized configuration
4. **TDD Gherkin Writer**: Create behavior-driven scenarios
5. **TDD Red Phase Tester**: Write failing tests
6. **TDD Green Phase Implementer**: Make tests pass
7. **TDD Refactor Phase Specialist**: Improve code quality
8. **Feature Builder**: Implement new features
9. **Code Maintainer**: Debug and maintain code
10. **Git Manager**: Control version control operations

## 🔍 Troubleshooting

### Visionary Recruiter Not Showing Up

If the Visionary Recruiter mode is not appearing in Roo Code:

1. Check the `.roomodes` file format:
   - It should contain a JSON object with a `customModes` array
   - The array should include the Visionary Recruiter configuration

2. Verify the mode definition:
   - Ensure `.roo/modes/visionary-recruiter.json` exists and is properly formatted
   - Check that the `slug` matches the reference in `.roomodes`

3. Restart Roo Code or VS Code

### Rule Files Not Being Applied

If the rule files are not being applied to the Visionary Recruiter:

1. Check the directory structure:
   - Rules should be in `.roo/rules-visionary-recruiter/`
   - Follow the naming convention: `XX_rule_name.md`

2. Verify file content:
   - Each rule file should have a clear title and content
   - Follow the format in the existing rule files

## 📚 Additional Resources

- [Roo Code Documentation](https://docs.roo.ai)
- [Custom Modes Guide](https://docs.roo.ai/custom-modes)
- [Model Context Protocol (MCP)](https://docs.roo.ai/mcp)