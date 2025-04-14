# Roo Crew: AI Agent Team Builder

This repository provides a framework for creating a comprehensive team of AI agents tailored to your specific project requirements. It allows you to define, configure, and deploy specialized AI agents that work together seamlessly to build and maintain your software project.

## Overview

The Roo Crew framework consists of two main components that work in sequence:

1. **Agent Team Generation**: Using the 🧠 Visionary Recruiter to create a specialized team of AI agents based on your project requirements.

2. **YAML Workflow Documentation**: Using the 📋 YAML Architect to create detailed step-by-step workflow documentation that assigns tasks to the specific agents created in the first phase.

This two-phase approach ensures that the YAML workflow documentation is tailored to your specific agent team, with each task assigned to the most appropriate specialized agent based on their expertise and responsibilities.

## Getting Started

### Prerequisites

- A modern LLM with agent capabilities (recommended: **Gemini 2.5** or **Claude 3.7**)
- Basic understanding of software development concepts
- A clear idea of your project requirements

## Phase 1: Agent Team Generation

This phase focuses on creating your specialized team of AI agents based on your project requirements.

### Steps:

1. **Clone this repository**:
   ```bash
   git clone https://github.com/yourusername/roo-crew.git
   cd roo-crew
   ```

2. **Customize the recruitment prompt**:
   - Open `prompt_recruitment.md` in your editor
   - Follow the instructions to select your technology stack, architectural patterns, and team structure
   - Customize the sections to match your project's specific requirements

3. **Generate your agent team**:
   - Use the 🧠 **Visionary Recruiter** mode to process your recruitment prompt
   - Run the following command in your LLM interface:
   ```
   Please analyze the prompt_recruitment.md file and generate a complete agent team definition based on the specified requirements.
   ```

4. **Implement the generated team**:
   - Follow the instructions provided by the Visionary Recruiter
   - Create the necessary agent definition files in the `.roomodes` file
   - Set up the required rules and protocols in the `.roo/rules/` directory

## Phase 2: YAML Workflow Documentation

After your agent team is created, this phase focuses on generating detailed workflow documentation that assigns tasks to your specialized agents.

### Steps:

1. **Customize the YAML workflow prompt**:
   - Open `prompt_yaml_workflow.md` in your editor
   - Ensure it references your project's specific requirements and technology stack
   - Make sure the Docker-First Principle and Command Execution sections are properly configured

2. **Generate YAML workflow documentation**:
   - Use the 📋 **YAML Architect** mode to create comprehensive workflow documentation
   - Run the following command in your LLM interface:
   ```
   Please analyze the prompt_yaml_workflow.md file and generate complete YAML workflow documentation for the project, assigning tasks to the specialized agents created in Phase 1.
   ```

3. **Review and implement the workflows**:
   - The YAML Architect will create detailed YAML files in the `config/` directory
   - Each file will document a specific phase of the project with tasks assigned to your specialized agents
   - These workflows serve as the blueprint for implementing your project

## Using the Agent Team and Workflows

Once your agent team and workflow documentation are set up, you can:

1. **Assign tasks to specific agents** based on their expertise as defined in the YAML workflows
2. **Coordinate complex workflows** through the 🚀 Project Orchestrator
3. **Maintain consistent code quality** through the established rules and protocols
4. **Scale your team** by adding new specialized agents as needed

The YAML workflow documentation provides a detailed roadmap for your project, with each task assigned to the specific agent from your team who is best suited to handle it.

## Repository Structure

- `prompt_recruitment.md`: The main configuration file for defining your project requirements
- `prompt_yaml_workflow.md`: Configuration for generating YAML workflow documentation
- `.roomodes`: Defines the available agent modes and their capabilities
- `.roo/rules/`: Contains global rules that apply to all agents
- `.roo/rules-{agent-slug}/`: Contains specific rules for each agent type
- `config/`: Contains YAML workflow documentation files that assign tasks to your agents

## Required Changes to Prompt Files

### Changes to `prompt_yaml_workflow.md`

Add the following to the Docker-First Principle section (section 2.3, point 4):

```markdown
4. **Docker-First Principle**: You MUST assume that all development occurs within Docker containers. No direct installation of tools on the host system is permitted. All environment setup must be containerized. CRITICAL: ALL commands (npm, yarn, tests, builds, etc.) MUST be executed within Docker containers. Commands should be prefixed with appropriate Docker or Docker Compose commands (e.g., `docker-compose exec`, `docker run`). The development container should be built at the beginning of the project in development mode, used throughout the development process, and only at the end should production containers be created.
```

Add a new point after Git Integration (section 2.3, point 6):

```markdown
6. **Command Execution**: Before executing any workflow, the YAML Architect MUST read and understand all YAML configuration files in the config/ directory to ensure adherence to established patterns and avoid inconsistencies.
```

### Changes to `prompt_recruitment.md`

Ensure the Containerization section (section 1.6) includes Docker and Docker Compose as selected options, and that the Deployment Pipeline section (section 3.4) emphasizes containerization:

```markdown
**Containerization:** All components must be containerized using Docker or equivalent technology <!-- Consistent environments -->
```

## Agent Modes to Use

1. **🧠 Visionary Recruiter**: Use this mode first to create your agent team based on the `prompt_recruitment.md` file. This agent will design a comprehensive team structure tailored to your project's specific technology stack and requirements.

2. **📋 YAML Architect**: Use this mode after your agent team is defined to create detailed YAML workflow documentation based on the `prompt_yaml_workflow.md` file. This agent will produce comprehensive step-by-step workflow files that assign tasks to the specialized agents created by the Visionary Recruiter.

3. **🚀 Project Orchestrator**: Once your team and workflows are defined, use this mode to coordinate tasks and delegate work to specialized agents according to the YAML workflow documentation.

## Example Workflow Files

The `config/` directory contains example YAML workflow files that demonstrate the expected structure and level of detail:

1. `example_01_project_initialization.yaml`: Project setup, repository initialization, and Docker environment configuration
2. `example_02_core_infrastructure.yaml`: Database schema, authentication system, UI component library, and API layer
3. `example_03_feature_development.yaml`: Dashboard layout, visualizations, data processing, and custom features
4. `example_04_testing_quality_assurance.yaml`: Unit testing, integration testing, end-to-end testing, performance testing, and security testing
5. `example_05_deployment_monitoring.yaml`: CI/CD pipeline, environment setup, monitoring, logging, and backup procedures

These files provide a real-world example with detailed steps that demonstrate the level of precision expected from the YAML Architect. Each step is assigned to a specific agent role from the team created by the Visionary Recruiter, ensuring that tasks are handled by the most appropriate specialized agent.

## Best Practices

1. **Be specific in your technology selections** - The more precise you are about your tech stack, the better tailored your agent team will be.

2. **Follow the TDD workflow** - The agents are designed to work in a test-driven development environment.

3. **Maintain centralized configuration** - All configuration should be managed through a single source of truth.

4. **Document everything** - Ensure comprehensive documentation is maintained throughout the project lifecycle.

5. **Use the confirmation gate** - Always confirm before pushing changes to the repository.

6. **Enforce containerization** - All development and testing should occur within Docker containers to ensure consistency.

## LLM Recommendations

This framework works best with advanced LLMs that support agent capabilities:

- **Gemini 2.5** (Recommended): Excellent at understanding complex instructions and generating structured outputs
- **Claude 3.7** (Recommended): Strong reasoning capabilities and good at following detailed protocols
- **GPT-4o**: Good alternative with strong coding capabilities

## Contributing

Contributions to improve the Roo Crew framework are welcome! Please feel free to submit pull requests or open issues to suggest improvements.

## License

This project is licensed under the MIT License - see the LICENSE file for details.