```markdown
# AGENTS.md File Guidelines

These guidelines are designed to ensure the development of AI coding agents within this repository adhere to best practices, promoting maintainability, testability, and overall quality.

## 1. DRY (Don't Repeat Yourself)

*   **Single Responsibility Principle:** Each agent should have a single, well-defined purpose. Avoid creating multiple agents with overlapping functionality.
*   **Component Reusability:** Components should be designed to be reusable across multiple agents or projects.
*   **Abstraction:**  Use abstract classes and interfaces to decouple components and promote flexibility.
*   **Consistent Design:**  Maintain a consistent design pattern across all agents.

## 2. KISS (Keep It Simple, Stupid)

*   **Minimize Complexity:**  Keep agent logic as straightforward as possible.  Avoid unnecessary features or convoluted algorithms.
*   **Readability:**  Code should be easily understood by other developers (including yourself in the future).
*   **Clear Naming:**  Use descriptive names for variables, functions, and classes.
*   **Avoid Over-Engineering:**  Don’t introduce complexity unless it demonstrably improves performance or maintainability.

## 3. SOLID Principles

*   **Single Responsibility:** (Reiterate) Each component should do one thing and do it well.
*   **Open/Closed Principle:**  The agent's core logic should be easily extensible through well-defined interfaces, not through modifying the core code itself.
*   **Liskov Substitution Principle:**  Subclasses should be substitutable for their base classes without altering the correctness of the program.
*   **Interface Segregation Principle:** Clients should not be forced to implement interfaces they do not use.
*   **Dependency Inversion Principle:**  High-level modules (agents) should not depend on low-level modules (interfaces).  Interfaces should define contracts.

## 4. YAGNI (You Aren’t Gonna Need It)

*   **Avoid Future Functionality:**  Don’t implement features that are not currently required.  Focus on the current task.
*   **Reactive Design:** Implement reactive systems with a clear understanding of the expected state transitions.
*   **Consider the Future:**  While not every detail needs to be planned, be mindful of potential future requirements.

## 5. Code Quality & Structure

*   **Line Length:**  Maximum 180 lines of code per file.
*   **Comments:**  Provide clear and concise comments where necessary to explain complex logic.
*   **Modularization:**  Break down large functions into smaller, more manageable units.
*   **Error Handling:** Implement basic error handling (e.g., exceptions) to gracefully handle unexpected situations.
*   **Documentation:**  Include a README file explaining the purpose, usage, and dependencies of each agent.
*   **Testability:** All agent logic must be testable via unit or integration tests.

## 6. Test Coverage

*   **Target 80%:**  The code must achieve at least 80% test coverage.
*   **Unit Tests:**  Prioritize writing comprehensive unit tests for each agent and component.
*   **Test-Driven Development (TDD):**  Consider implementing TDD practices to drive development.
*   **Mocking:**  Use mocks and stubs sparingly, *only* for unit tests.  Avoid mocking internal implementation details.

## 7. File Structure & Conventions

*   **Consistent Directory Structure:**  Organize files into logical directories reflecting the agent's functionality.
*   **File Naming Conventions:**  Use a consistent naming scheme for files and classes.
*   **API Documentation:**  For each agent, include a brief API documentation (e.g., using Swagger/OpenAPI) to explain the available functions and parameters.
*   **Dependency Management:**  Use a dependency management tool (e.g., `pip`, `poetry`) to track dependencies.

## 8.  General Considerations

*   **Code Reviews:**  All code should be reviewed by at least one other developer to identify potential issues.
*   **Version Control:** Use a version control system (e.g., Git) to track changes.
*   **Regular Updates:**  Review and update the code as needed to maintain its quality and relevance.
*   **Documentation Updates:**  Update documentation whenever a significant change is made to the agent's functionality.

```