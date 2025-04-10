# STANDING ORDER 02: SECURITY PROTOCOLS

## CLASSIFICATION: GLOBAL DIRECTIVE - ALL UNITS

All agents must implement and enforce comprehensive security measures throughout the codebase. Security is a non-negotiable priority that supersedes all other considerations except core functionality.

## TACTICAL EXECUTION POINTS:

1. **Strict Input Validation**: All user inputs MUST be validated and sanitized before processing. Implement type checking, range validation, and pattern matching for all inputs regardless of source. Reject any input that does not conform to expected patterns.

2. **Authentication & Authorization**: Implement proper authentication for all user actions and enforce strict authorization checks for all protected resources. Use industry-standard authentication protocols and maintain clear separation between authentication and authorization logic.

3. **Data Protection**: All sensitive data MUST be encrypted both in transit and at rest. Use strong, industry-standard encryption algorithms and proper key management. Never store sensitive data in logs, client-side storage, or version control.

4. **Dependency Security**: Regularly audit and update all dependencies. Implement automated vulnerability scanning in the CI/CD pipeline. Block deployment of any code with known vulnerable dependencies.

5. **Security by Design**: Incorporate security considerations from the beginning of feature development. Conduct threat modeling for all new features and document potential attack vectors along with mitigation strategies.

6. **Error Handling**: Implement secure error handling that prevents information leakage. Never expose stack traces, system information, or sensitive data in error messages presented to users.

SECURITY BREACHES RESULTING FROM NON-COMPLIANCE WITH THESE PROTOCOLS WILL BE TREATED AS CRITICAL FAILURES.