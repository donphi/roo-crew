# Roo Crew: AI Agent Team Builder

This repository provides a framework for creating a comprehensive team of AI agents tailored to your specific project requirements. It allows you to define, configure, and deploy specialized AI agents that work together seamlessly to build and maintain your software project.

## Getting Started

### Prerequisites

- A modern LLM with agent capabilities (recommended: **Gemini 2.5** or **Claude 3.7**)
- Basic understanding of software development concepts
- A clear idea of your project requirements

### Setup Process

1. **Clone this repository**:
   ```bash
   git clone https://github.com/yourusername/roo-crew.git
   cd roo-crew
   ```

2. **Customize the recruitment prompt**:
   - Open `.recruitment_prompt` in your editor
   - Follow the instructions to select your technology stack, architectural patterns, and team structure
   - Customize the sections to match your project's specific requirements

3. **Generate your agent team**:
   - Use the Visionary Recruiter mode to process your recruitment prompt
   - Run the following command in your LLM interface:
   ```
   Please analyze the .recruitment_prompt file and generate a complete agent team definition based on the specified requirements.
   ```

4. **Implement the generated team**:
   - Follow the instructions provided by the Visionary Recruiter
   - Create the necessary agent definition files
   - Set up the required rules and protocols

## Using the Agent Team

Once your agent team is set up, you can:

1. **Assign tasks to specific agents** based on their expertise
2. **Coordinate complex workflows** through the Project Orchestrator
3. **Maintain consistent code quality** through the established rules and protocols
4. **Scale your team** by adding new specialized agents as needed

## Repository Structure

- `.recruitment_prompt`: The main configuration file for defining your project requirements
- `.roomodes`: Defines the available agent modes and their capabilities
- `.roo/rules/`: Contains global rules that apply to all agents
- `.roo/rules-{agent-slug}/`: Contains specific rules for each agent type

## Best Practices

1. **Be specific in your technology selections** - The more precise you are about your tech stack, the better tailored your agent team will be.

2. **Follow the TDD workflow** - The agents are designed to work in a test-driven development environment.

3. **Maintain centralized configuration** - All configuration should be managed through a single source of truth.

4. **Document everything** - Ensure comprehensive documentation is maintained throughout the project lifecycle.

5. **Use the confirmation gate** - Always confirm before pushing changes to the repository.

## LLM Recommendations

This framework works best with advanced LLMs that support agent capabilities:

- **Gemini 2.5** (Recommended): Excellent at understanding complex instructions and generating structured outputs
- **Claude 3.7** (Recommended): Strong reasoning capabilities and good at following detailed protocols
- **GPT-4o**: Good alternative with strong coding capabilities

## Contributing

Contributions to improve the Roo Crew framework are welcome! Please feel free to submit pull requests or open issues to suggest improvements.

## License

This project is licensed under the MIT License - see the LICENSE file for details.