# YAML WORKFLOW DOCUMENTATION REQUEST
==================================================================================================

## SECTION 1: PROJECT DEFINITION
--------------------------------------------------------------------------------------------------

### 1.1 CLASSIFICATION
MISSION CRITICAL

### 1.2 AUTHORIZATION
TO: YAML ARCHITECT AGENT
FROM: PROJECT COMMANDER
SUBJECT: COMPREHENSIVE PROJECT WORKFLOW DOCUMENTATION

### 1.3 PROJECT TYPE
[USER: SELECT ONE]
- Minimum Viable Product (MVP)
- Full Production Project
- Proof of Concept
- Technical Prototype
- Maintenance/Enhancement of Existing System
- Migration Project
- Research & Development

### 1.4 PROJECT SCOPE AND OBJECTIVES
[USER: REPLACE THIS SECTION WITH YOUR DETAILED PROJECT DESCRIPTION]

Provide a comprehensive description of your project including:
1. The problem the project aims to solve
2. The target users/audience
3. Key features and functionality required
4. Specific business requirements
5. Technical constraints or requirements
6. Success criteria and definition of "done"
7. Any specific milestones or phases
8. Performance expectations
9. Security requirements
10. Scalability considerations

Be as detailed as possible about the end state of the project. The more specific information you provide here, the more precise and useful the generated workflow will be.

### 1.5 MISSION BRIEFING

You are ORDERED to create a comprehensive set of YAML workflow documents that will serve as the definitive blueprint for executing the project defined in the PROJECT SCOPE AND OBJECTIVES section above and the technology stack defined in the `prompt_recruitment.md` file. These documents must capture every single step, decision point, validation checkpoint, and error handling procedure required to successfully implement the project from inception to deployment.

## SECTION 2: WORKFLOW ORGANIZATION
--------------------------------------------------------------------------------------------------

### 2.1 TECHNOLOGY MODULES
Your workflow documentation MUST be organized into distinct technology modules, each with its own numbered steps:

1. **Frontend Module**: All steps related to UI/UX, frontend frameworks, client-side logic
   - Numbered steps: FRONT-001, FRONT-002, etc.

2. **Backend Module**: All steps related to server-side logic, APIs, business logic
   - Numbered steps: BACK-001, BACK-002, etc.

3. **Database Module**: All steps related to data modeling, storage, migrations
   - Numbered steps: DB-001, DB-002, etc.

4. **DevOps Module**: All steps related to CI/CD, deployment, infrastructure
   - Numbered steps: DEVOPS-001, DEVOPS-002, etc.

5. **Testing Module**: All steps related to testing at various levels
   - Numbered steps: TEST-001, TEST-002, etc.

6. **Documentation Module**: All steps related to documentation creation and maintenance
   - Numbered steps: DOC-001, DOC-002, etc.

7. **Integration Module**: All steps related to integrating different components
   - Numbered steps: INT-001, INT-002, etc.

### 2.2 WORKFLOW FILE LOCATION
All workflow YAML files MUST be stored in the `config/` directory of the project. This ensures centralization of all workflow documentation and makes it easily discoverable.

### 2.3 WORKFLOW PHASES
Within each technology module, organize steps according to these sequential phases:

1. **Phase 1: Project Initialization** (File: `config/01_project_initialization.yaml`)
   - Environment setup
   - Repository initialization
   - Initial architecture scaffolding
   - Centralized configuration system establishment

2. **Phase 2: Core Infrastructure Development** (File: `config/02_core_infrastructure.yaml`)
   - Database schema design and implementation
   - Authentication/authorization system
   - Core API structure
   - Reusable component/template library

3. **Phase 3: Feature Development** (File: `config/03_feature_development.yaml`)
   - Feature-by-feature implementation process
   - TDD workflow for each feature
   - Documentation requirements
   - Code review process

4. **Phase 4: Testing & Quality Assurance** (File: `config/04_testing_quality_assurance.yaml`)
   - Unit testing procedures
   - Integration testing procedures
   - End-to-end testing procedures
   - Performance testing (if applicable)
   - Security testing

5. **Phase 5: Deployment & Monitoring** (File: `config/05_deployment_monitoring.yaml`)
   - CI/CD pipeline configuration
   - Environment setup (dev, staging, production)
   - Monitoring and logging implementation
   - Backup and disaster recovery procedures

### 2.3 OPERATIONAL PARAMETERS

1. **Technology Stack Analysis**: You MUST first analyze the `prompt_recruitment.md` file to extract the complete technology stack, architectural requirements, and operational protocols specific to this project.

2. **Agent Integration**: You MUST incorporate ALL custom agent modes created by the Visionary Recruiter. You are FORBIDDEN from using the default "code", "architect", "ask", or "debug" modes. Only custom modes defined in the `.roomodes` file are authorized for inclusion in the workflow.

3. **Project Orchestrator Centrality**: EVERY workflow MUST begin with the Project Orchestrator agent. No action can be initiated without the Project Orchestrator's explicit delegation and oversight.

4. **Docker-First Principle**: You MUST assume that all development occurs within Docker containers. No direct installation of tools on the host system is permitted. All environment setup must be containerized. CRITICAL: ALL commands (npm, yarn, tests, builds, etc.) MUST be executed within Docker containers. Commands should be prefixed with appropriate Docker or Docker Compose commands (e.g., `docker-compose exec`, `docker run`). The development container should be built at the beginning of the project in development mode, used throughout the development process, and only at the end should production containers be created.

5. **Git Integration**: All workflows must include appropriate Git operations with the mandatory confirmation gate before any push operations.

6. **Command Execution**: Before executing any workflow, the YAML Architect MUST read and understand all YAML configuration files in the config/ directory to ensure adherence to established patterns and avoid inconsistencies.

## SECTION 3: STEP STRUCTURE REQUIREMENTS
--------------------------------------------------------------------------------------------------

### 3.1 YAML STRUCTURE TEMPLATE

Each workflow step MUST include the following information, with a clear status marker at the left of each step:

```yaml
steps:
  - id: "MODULE-NNN"  # e.g., FRONT-001, BACK-003, etc.
    status_marker: "[ ]"  # Must be one of: "[ ]" (not started), "[P]" (pending), "[✓]" (complete), "[!]" (error)
    name: "Clear, descriptive name of the step"
    description: "Extremely detailed description of what this step accomplishes and why it's necessary"
    status: "not_started"  # Options: not_started, pending, complete, error
    error_details: ""  # Required if status is "error", must explain exactly what went wrong
    phase: 1  # Corresponding to the phase number (1-5)
    
    orchestrator:
      action: "delegate"  # The Project Orchestrator always initiates by delegating
      rationale: "Detailed explanation of why this specific agent was selected for this task"
    
    assigned_to: "agent-slug"  # Must be a valid agent slug from .roomodes
    estimated_time: "X hours/minutes"
    
    technology_stack:
      # List all specific technologies from prompt_recruitment.md relevant to this step
      primary_language: "Selected language from recruitment prompt"
      frameworks: ["Framework1", "Framework2"]
      tools: ["Tool1", "Tool2"]
    
    prerequisites:
      environment:
        - "Docker must be running"
        - "Other specific environmental requirements"
      knowledge:
        - "Specific knowledge areas required"
      resources:
        - "Specific resources needed"
      dependencies:
        - "step-id-of-prerequisite-step"
    
    development_approach:
      tdd_required: true/false  # Based on prompt_recruitment.md
      pair_programming: true/false  # For complex features
      documentation_update_required: true/false
    
    adherence_requirements:
      - "Specific architectural principles from prompt_recruitment.md that must be followed"
      - "Specific code organization requirements"
      - "Specific design patterns to implement"
    
    validation:
      criteria:
        - "Specific, measurable criteria that indicate successful completion"
      commands:
        - "Exact commands to validate success"
    
    error_handling:
      potential_errors:
        - error: "Potential error description"
          detection: "How to detect this error"
          resolution: "Specific steps to resolve this error"
      
    git_operations:
      required: true/false
      confirmation_required: true/false  # Always true for push operations
      
    substeps:
      # Recursive structure for more granular steps
      - id: "MODULE-NNN.1"  # e.g., FRONT-001.1, BACK-003.2, etc.
        status_marker: "[ ]"  # Must be one of: "[ ]" (not started), "[P]" (pending), "[✓]" (complete), "[!]" (error)
        # Same structure as parent steps
```

The status_marker field is CRITICAL as it provides a clear visual indicator of step completion status that agents can easily update. This marker MUST be prominently displayed at the beginning of each step and substep.

## SECTION 4: EXECUTION REQUIREMENTS
--------------------------------------------------------------------------------------------------

### 4.1 QUALITY STANDARDS

1. **Absolute Precision**: Every step must be documented with such precision that it could be executed by someone with minimal technical knowledge or by an automated system.

2. **Technology Specificity**: All steps must reference the EXACT technologies specified in the `prompt_recruitment.md` file. Generic instructions are FORBIDDEN.

3. **Error Anticipation**: Every step must include comprehensive error handling with specific detection methods and resolution procedures.

4. **Validation Gates**: Every major step must include explicit validation criteria and commands to verify successful completion before proceeding.

5. **Agent Specialization**: Tasks must be assigned to agents based on their specific expertise and responsibilities as defined in the `.roomodes` file.

6. **Single Agent Focus**: Only one agent can work on a specific subtask at a time. If an agent cannot complete a task, it must be explicitly returned to the Project Orchestrator for reassignment.

### 4.2 DELIVERABLES

You MUST produce a set of YAML files (maximum 5) that collectively document the entire project workflow from initialization to deployment. These files must be so comprehensive and precise that they could serve as the sole reference for implementing the entire project.

FAILURE TO PROVIDE THIS LEVEL OF DETAIL AND PRECISION WILL RESULT IN MISSION FAILURE.

### 4.3 EXECUTION COMMAND

To create these workflow documents, you must:

1. Analyze the `prompt_recruitment.md` file to understand the project requirements, technology stack, and architectural directives
2. Identify all custom agent modes from the `.roomodes` file
3. Create the workflow YAML files with the structure specified above
4. Ensure all steps are assigned to appropriate specialized agents
5. Verify that all workflows begin with the Project Orchestrator
6. Confirm that all steps include comprehensive error handling and validation

BEGIN EXECUTION IMMEDIATELY.