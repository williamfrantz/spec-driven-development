# Spec Driven Development Rules for Amazon Q Developer

A methodical approach to software development that prevents rushing to code without proper planning, requirements, and design.

## Philosophy

Most software projects fail not because of poor coding, but because of poor planning. Developers with AI coding assistants often jump straight to implementation without understanding the problem, gathering requirements, or designing a solution. This leads to:

- Features that don't solve the actual problem
- Code that's hard to maintain and extend  
- Missed requirements discovered late in development
- Technical debt from hasty architectural decisions
- Frustration from constant rework and refactoring

**Spec Driven Development** addresses these issues by enforcing a structured, phase-based approach where each phase must be completed and approved before moving to the next. This methodology works particularly well with AI coding assistants like Amazon Q Developer, which excel at following systematic processes.

## How It Works

The rules define five distinct phases with clear boundaries:

### Phase 1: Concepts and Brainstorming
- Explore and refine the core idea
- Document the chosen concept

### Phase 2: Requirements  
- Write detailed user stories with acceptance criteria
- Use EARS format (Easy Approach to Requirements Syntax)
- Get explicit approval before proceeding

### Phase 3: Design
- Research technical challenges and solutions
- Create comprehensive technical specifications
- Address architecture, components, data models, and error handling

### Phase 4: Implementation Planning
- Break design into specific, actionable coding tasks
- Create step-by-step prompts for AI coding assistants
- Ensure incremental, test-driven development approach

### Phase 5: Development
- Execute the implementation plan methodically
- Complete one task at a time with validation
- Maintain traceability back to requirements

## Key Benefits

- **Prevents Feature Creep**: Clear requirements and approval gates
- **Reduces Rework**: Thorough planning catches issues early
- **Improves Code Quality**: Test-driven, incremental approach
- **Better Documentation**: Living specs that stay current
- **Junior Developer Friendly**: Clear, unambiguous instructions
- **AI Assistant Optimized**: Structured prompts and systematic processes

## Operating Modes

The rules define three operating modes that control what the AI assistant can modify:

- **Planning Mode**: Read-only
- **Documenting Mode**: Can create/modify Markdown documentation only  
- **Implementing Mode**: Full file system access for coding

This prevents premature implementation and ensures proper documentation.

## Installation

### For Amazon Q Developer CLI

1. Navigate to your project root directory
2. Create the Amazon Q rules directory:
   ```bash
   mkdir -p .amazonq/rules
   ```

3. Copy the rules file:
   ```bash
   curl -o .amazonq/rules/spec-driven-development.md https://raw.githubusercontent.com/williamfrantz/spec-driven-development/main/spec-driven-development.md
   ```

   Or manually download and place `spec-driven-development.md` in `.amazonq/rules/`

4. Launch Amazon Q from your project directory:
   ```bash
   q chat
   ```

5. Alternatively, open Visual Studio Code with the Amazon Q Developer extension in a folder containing `.amazonq/rules/spec-driven-development.md`

Either version of Amazon Q will automatically load and apply these rules every time it's launched from a directory containing `.amazonq/rules/`.

### For Other AI Assistants

While designed for Amazon Q Developer, these rules can be adapted for other AI coding assistants:

1. Copy the contents of `spec-driven-development.md`
2. Paste into your AI assistant's custom instructions or system prompt
3. Modify any Amazon Q-specific references as needed

## Examples

### Quick Start Example
```
"I want to add a user authentication feature to my web application. Let's start with the concept and requirements."
```

### Multi-Feature Project
```
"I'm building a task management app. Let's define the overall concept and then work through requirements for user registration, task creation, and task assignment features."
```

## Troubleshooting

**Q: Amazon Q isn't following the rules**
- Ensure the file is in `.amazonq/rules/spec-driven-development.md`
- Restart Amazon Q from the project directory
- Verify the file contains the complete rule set

**Q: Can I use this with other AI assistants?**
- Yes! Copy the rules content into your AI assistant's custom instructions
- You may need to adapt Amazon Q-specific references

**Q: What if I need to change requirements mid-project?**
- The rules allow returning to previous phases when needed
- Update the requirements document and get approval before proceeding
- Implementation plans can be revised based on updated requirements

## Version History

- **v1.0** - Initial release with five-phase development process

## Contributing

This is an evolving methodology. Contributions, improvements, and real-world feedback are welcome:

1. Fork this repository
2. Create a feature branch for your improvements
3. Test the changes with actual projects
4. Submit a pull request with your rationale

## License

MIT License - Feel free to use, modify, and distribute these rules for your projects.

