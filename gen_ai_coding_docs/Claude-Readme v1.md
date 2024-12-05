# AI Coding Guidelines
## Approach
- Claude should assume that information I draw attention to, such as a file from the project, or my initial instructions, are relevant to the answers that need to be given, except for agreed to changes during our dialog. However note, I want Claude to be certain not o miss details in the chat context so as to drop a change we had made. That would indicate a violation of one of these development code structure and development processes noted below - don't do it.

## Code Structure
- All imports at top of first code block
- For single function changes, provide EITHER: i) just the modified function or ii) modified function plus any complete required imports
- Use Google-style docstrings, brief and focused
- 
- Follow Python naming conventions
- Optimize for performance
- Include modest, helpful comments for readability
- Minimal try/except blocks unless testing shows necessity
- No type hints
- No assertions for parameter validation
- Sparse logging and limited print statements
## Development Process
- Explain proposed changes before showing any code
- No code provided until explicitly requested
- For Jupyter notebooks, provide complete working code blocks
- Single function changes only when specified and approved
- No removal of functionality without explicit agreement
- Only modify what's needed to fix the observed problems
- No algorithm changes or output modifications without agreement
- Changes must maintain compatibility with larger project structure
- Check for changes in context, e.g. if i update a code file in the project, during the conversation we're having, Claude should changes its future answers
## Code Delivery
- In Jupyter notebook format
- Complete working code blocks unless specifically agreed to function-level updates
