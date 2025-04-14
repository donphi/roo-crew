# STANDING ORDER 05: PROCESS VALIDATION

## CLASSIFICATION: QUALITY ASSURANCE PROTOCOL

You are COMMANDED to design all YAML process documentation with built-in validation mechanisms that allow for systematic testing and verification of the entire process. Every documented workflow must be inherently testable. This directive is NON-NEGOTIABLE.

## TACTICAL EXECUTION POINTS:

1. **Testability By Design**: Structure all processes so they can be validated through automated testing, with clearly defined inputs, expected outputs, and success criteria for each step and the overall process.

2. **Validation Checkpoints**: Insert explicit validation steps at critical junctures in the process that verify:
   - Preconditions are met before proceeding
   - Expected intermediate states are achieved
   - Resources are properly allocated and accessible
   - Output meets quality and correctness criteria

3. **Idempotency Considerations**: Design processes to be idempotent where possible, ensuring that repeated execution does not cause unintended side effects, and document explicit checks for detecting and handling partial completion states.

4. **Dry-Run Capability**: Include a specific "dry run" or simulation mode for each process that allows validation of the entire workflow without making permanent changes to production systems.

5. **Rollback Procedures**: Define comprehensive rollback procedures for each major step that can restore the system to its previous state if validation fails, including:
   - Backup procedures before state-changing operations
   - Specific commands or actions to revert changes
   - Verification steps to confirm successful rollback

6. **End-to-End Validation**: Conclude each process with a comprehensive end-to-end validation that confirms the entire workflow achieved its intended purpose, with specific tests for all success criteria.

PROCESSES THAT CANNOT BE SYSTEMATICALLY VALIDATED ARE FUNDAMENTALLY FLAWED AND POSE UNACCEPTABLE OPERATIONAL RISKS. NO EXCEPTIONS.