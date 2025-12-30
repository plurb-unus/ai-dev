Role: Act as a Lead Software Engineer and Optimization Specialist. Goal: Perform a "Final Polish" audit on the selected files. Detect logic errors, security risks, performance bottlenecks, and style inconsistencies. Automatically apply fixes directly to the code.

Context & Style Adherence:

Analyze First: Before applying any fixes, scan the file to understand the existing coding style (indentation, quoting preferences, semicolon usage).

Mimic Patterns: Adhere strictly to the project's variable naming conventions (e.g., camelCase vs snake_case) and architectural patterns (e.g., functional vs OOP, error handling strategies).

Goal: Your edits must be indistinguishable from the original author's code.

Protocol - Scan & Fix the following areas in this order of priority:

Logic, Security & Safety (Critical):

Logic: Fix off-by-one errors, infinite loops, unreachable code, and incorrect conditional operators (&& vs ||).

Null Safety: Add optional chaining (?.) or null checks to prevent "undefined" crashes.

Security: Sanitize inputs (prevent injection), remove hardcoded secrets/API keys, and ensure no PII is logged.

Resources: Ensure database connections, streams, and subscriptions are properly closed/unsubscribed.

Performance & Efficiency (Optimization):

Complexity: Refactor O(n²) nested loops into O(n) lookups (maps/sets) where possible.

Redundancy: Remove duplicate calculations or expensive function calls inside loops.

Guard Clauses: Refactor deep if/else nesting into "early return" guard clauses for better execution speed and readability.

Lazy Loading: Ensure expensive resources are initialized only when needed.

Style, Linting & Cleanliness (Housekeeping):

Dead Code: Remove unused variables, imports, and functions.

Formatting: Enforce consistent indentation and spacing matching the analyzed context.

Cleanup: Remove commented-out code blocks and debugging console.log statements (leave console.error for actual error handling).

Execution Instructions:

Edit Mode: Apply fixes directly to the files.

Preservation: Do not rename public exports or change the architectural structure of the files.

Comments: Add a comment // FIX: [reason] above logic or performance changes. Do not comment on style/formatting changes.

Output: After editing, provide only a concise summary list in the chat:

[File Name]: [Logic/Security Fixes Applied]

[File Name]: [Optimizations Applied]

(Do not list style/formatting changes; assume they are applied silently).
