# AI Coding Guidelines

## Introduction
This document outlines guidelines for coding projects with Claude. Include this readme within projects when creating or modifying codebases.

## Environment
- Python 3.13 unless project specifies otherwise
- Jupyter notebooks for code delivery
- Latest version of libraries unless specified
- Windows, VS Code (with Markdown Preview, Pylance, Python, GitLens, Jupyter extensions)
- Virtual environments required

## Code Structure
- All imports at top of first code block
- For single function changes: provide either modified function alone or with required imports
- Follow Google Python Style Guide (https://google.github.io/styleguide/pyguide.html)
- Use Google-style docstrings, brief and focused
- Follow Python naming conventions
- Optimize for performance
- Comments:
  - 1-2 lines explaining function purpose
  - Single line explanations for complex loops/conditionals
- Minimal try/except blocks unless testing shows necessity
- No type hints
- No assertions for parameter validation
- Print statements limited to:
  - Troubleshooting
  - Critical progress notifications
  - Task completion confirmation
- Remove deprecated code with brief explanatory note

## Development Process
- Explain proposed changes before showing code
- No code provided until explicitly requested
- Only modify what's needed to fix observed problems
- Prefer single-function changes over reworking multiple functions
- Notify before making larger changes (multiple files/significant algorithm changes)
- Present change overview in English and await approval
- No removal of functionality without explicit agreement
- No algorithm changes or output modifications without agreement
- Changes must maintain compatibility with larger project structure
- Check for changes in context during conversations
- Request guidance for dependency updates
- Notify when readme/docstring updates may be needed

## Testing Requirements
- Write unit tests for new functions
- Update existing tests for modified functions
- Minimum test coverage: 80% for new code
- Include positive and negative test cases
- Test edge cases and error conditions
- Document test assumptions in test docstrings

## Code Delivery
- In Jupyter notebook format
- Complete working code blocks unless specifically agreed to function-level updates

## Response Format
- Use numbered sequence (1, 2, 3, etc.)
- Use sub-numbering for details (1.1, 1.2, 1.3, etc.)
- No bullets or roman numerals
- Prefer concise responses


## Document History
- 2024-12-05: v2.0 - Updated from previous after dialogue from Claude