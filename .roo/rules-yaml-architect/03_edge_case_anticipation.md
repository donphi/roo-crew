# STANDING ORDER 03: EDGE CASE ANTICIPATION

## CLASSIFICATION: RISK MITIGATION PROTOCOL

You are COMMANDED to anticipate and document ALL possible edge cases, failure modes, and exception scenarios for every process you document. No step is complete without comprehensive error handling and recovery procedures. This directive is ABSOLUTE.

## TACTICAL EXECUTION POINTS:

1. **Exhaustive Error Cataloging**: For each atomic step, identify and document all possible failure modes, including but not limited to: resource unavailability, permission issues, timeout scenarios, data validation failures, and unexpected state conditions.

2. **Conditional Branching**: Implement explicit conditional logic for each identified edge case, with clear decision criteria and separate execution paths for normal operation versus exception handling.

3. **Recovery Procedures**: Define specific, actionable recovery steps for each failure mode, including:
   - Immediate mitigation actions
   - Diagnostic information to collect
   - Retry strategies with backoff parameters
   - Escalation thresholds and procedures
   - Rollback operations to restore system to known-good state

4. **Validation Gates**: Insert validation checkpoints after critical operations that verify expected outcomes before proceeding, with explicit handling for validation failures.

5. **Graceful Degradation**: Where appropriate, document procedures for continuing operation in degraded mode when full recovery is not immediately possible.

6. **Monitoring Hooks**: Specify monitoring points throughout the process where status should be logged, metrics collected, and alerts potentially triggered.

FAILURE TO ANTICIPATE EDGE CASES WILL RESULT IN BRITTLE PROCESSES THAT COLLAPSE UNDER REAL-WORLD CONDITIONS. COMPREHENSIVE EXCEPTION HANDLING IS NOT OPTIONAL.