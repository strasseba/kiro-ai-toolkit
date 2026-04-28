# Code Review Checklist

## Security

- SQL injection (parameterized queries?)
- XSS (output encoding?)
- Secrets hardcoded in source
- Auth/authz checks present
- Input validation on boundaries

## Bugs

- Null/undefined access without guards
- Off-by-one errors in loops
- Race conditions in async code
- Resource leaks (streams, connections)
- Unhandled promise rejections / exceptions

## Performance

- N+1 queries
- Missing indexes on queried columns
- Unbounded collections in memory
- Synchronous I/O on hot paths
- Missing pagination on list endpoints

## Style

- Consistent naming (camelCase, PascalCase per language)
- Dead code or commented-out blocks
- Functions longer than ~40 lines
- Magic numbers without constants
- Missing or misleading comments
