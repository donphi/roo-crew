# STANDING ORDER 04: IMPLEMENTATION CLARITY

## CLASSIFICATION: EXECUTION STANDARD

You are ORDERED to ensure that every step in your YAML documentation is described with such precision and clarity that it can be executed without ambiguity by either a human or an automated system. No room for interpretation or implicit knowledge is acceptable. This directive is INVIOLABLE.

## TACTICAL EXECUTION POINTS:

1. **Explicit Command Syntax**: When documenting technical operations, provide the exact command syntax, including all parameters, flags, and expected output patterns. For example, instead of "install the package," specify `npm install package-name@version --save-exact`.

2. **Environmental Prerequisites**: For each step or process, explicitly document all required environmental conditions, including:
   - Required software versions
   - System dependencies
   - Configuration settings
   - Resource requirements (memory, disk space, network access)
   - Required permissions and access levels

3. **Success Criteria**: Define unambiguous, measurable criteria for determining when a step has been successfully completed, preferably with automated verification methods where applicable.

4. **Input-Output Specifications**: For each step, precisely define:
   - Required input format, structure, and validation rules
   - Expected output format and structure
   - State changes that should result from execution
   - Side effects that may occur

5. **Visual Documentation**: Where appropriate, include diagrams, screenshots, or other visual aids that clarify complex procedures or expected visual outcomes.

6. **Executable Examples**: Provide complete, working examples for complex operations that can be directly copied and executed, with sample inputs and expected outputs.

AMBIGUITY IN DOCUMENTATION LEADS TO INCONSISTENT IMPLEMENTATION AND CASCADING FAILURES. ABSOLUTE PRECISION IS MANDATORY.