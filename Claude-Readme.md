# AI Coding Guidelines
## Approach
- Claude should assume that information I draw attention to, such as a file from the project, or my initial instructions, are relevant to the response required, except for changes agreed to during our dialog. However note, I want Claude to be certain not to miss details in the chat context so as to drop a change we had made. That would indicate a violation of one of these development code structure and development processes noted below - don't do it.

## Environment
- Unless otherwise specified, use Python 3.13
- Use Jupyter notebooks for code delivery
- Use the latest version of libraries unless otherwise specified
- Windows, VS Code, and Jupyter Notebook

## Code Structure
- All imports at top of first code block
- For single function changes, provide EITHER: i) just the modified function or ii) modified function plus any complete required imports
- Use Google-style docstrings, brief and focused
- 
- Follow Python naming conventions
- Optimize for performance
- Include minimal, helpful comments for readability
- Minimal try/except blocks unless testing shows necessity
- No type hints
- No assertions for parameter validation
- Sparse logging and limited print statements
## Development Process
- Explain proposed changes before showing any code
- No code provided until explicitly requested
- Only modify what's needed to fix the observed problems
- Prefer single-function changes over reworking multiple functions
- No removal of functionality without explicit agreement
- No algorithm changes or output modifications without agreement
- Changes must maintain compatibility with larger project structure
- Check for changes in context, e.g. if i update a code file in the project, during the conversation we're having, Claude should changes its future answers
## Code Delivery
- In Jupyter notebook format
- Complete working code blocks unless specifically agreed to function-level updates