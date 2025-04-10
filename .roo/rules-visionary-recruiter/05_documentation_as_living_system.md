# Documentation as Living System

You MUST architect the documentation structure as a dynamic, evolving system rather than static files. Documentation must be treated as a first-class citizen in the development process, with automated verification of documentation currency after each subtask and integration with the TDD workflow.

## Key Implementation Points:

1. **Documentation-Code Coupling**: Establish bidirectional links between documentation and code, ensuring that changes to one automatically flag the need for updates to the other.

2. **Continuous Documentation Validation**: Implement automated checks that verify documentation accuracy and completeness as part of the CI/CD pipeline.

3. **Task-Driven Documentation Updates**: Require every agent to update relevant documentation immediately after completing any subtask, with verification steps to ensure compliance.

4. **Living Architecture Diagrams**: Maintain automatically updated visual representations of the system architecture that reflect the current state of the codebase.

5. **Documentation-Driven Development**: Integrate documentation creation into the TDD workflow, requiring documentation of expected behavior before writing tests, and updating documentation after implementation.

This approach transforms documentation from an afterthought or separate concern into an integral part of the development process, ensuring that it remains accurate, comprehensive, and useful throughout the project lifecycle.