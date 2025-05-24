# 🧠 Prompt Labs Toolkit

A collection of reusable prompt templates for software development tasks.

---

## 🔧 Core Tools

### 1. `api_documenter`
**What:** Generates comprehensive API documentation  
**When to Use:** When documenting APIs or reviewing incomplete specs  
**Parameters:**  
```text
auto_followup: Write instructions as user requirements
```
**Example:**
```xml
<thinking>
User wants API documentation but missed parameter requirements, authentication, and error responses.
</thinking>
<prompt_tool>
<tool_name>api_documenter</tool_name>
<auto_followup>Please include base URL, required/optional parameters with defaults, request examples for JSON/form-data, status codes (200,400,401,403,500), and error response examples.</auto_followup>
</prompt_tool>
```

### 2. `architecture_advisor`
**What:** Evaluates architectural trade-offs  
**When to Use:** Designing system architecture or major features  
**Parameters:**  
```text
options: Provide 2-4 architectural options
```
**Example:**
```xml
<thinking>
User needs to choose architecture for a data-intensive app.
</thinking>
<prompt_tool>
<tool_name>architecture_advisor</tool_name>
<options>["Microservices with API Gateway", "Monolith with DDD", "Event-Driven", "Serverless"]</options>
</prompt_tool>
```

### 3. `code_refactor`
**What:** Guides code restructuring  
**When to Use:** Improving maintainability of complex code  
**Parameters:**  
```text
options: Provide 2-4 refactoring strategies
```
**Example:**
```xml
<thinking>
User has complex function with nested logic.
</thinking>
<prompt_tool>
<tool_name>code_refactor</tool_name>
<options>["Extract Helper Functions", "Apply Strategy Pattern", "Simplify Conditionals"]</options>
</prompt_tool>
```

### 4. `unit_test`
**What:** Guides test implementation  
**When to Use:** Writing or reviewing tests  
**Parameters:**  
```text
options: Provide testing framework/approach options
```
**Example:**
```xml
<thinking>
User needs test guidance for React component.
</thinking>
<prompt_tool>
<tool_name>unit_test</tool_name>
<options>["Jest with RTL", "Snapshot Testing", "Integration Tests with Mock API"]</options>
</prompt_tool>
```

### 5. `variable_namer`
**What:** Assists with clean variable names  
**When to Use:** Naming variables or improving code readability  
**Parameters:**  
```text
options: Specify naming task type
```
**Example:**
```xml
<thinking>
User needs help naming a user count variable.
</thinking>
<prompt_tool>
<tool_name>variable_namer</tool_name>
<options>["Suggest names for user count", "Explain JS naming conventions"]</options>
</prompt_tool>
```

---

## 📦 Additional Tools

| Tool              | Purpose                          | Key Use Case                          |
|-------------------|----------------------------------|---------------------------------------|
| `code_review`     | Structured code feedback         | Reviewing code quality/best practices |
| `commit_assistant`| Commit organization & messages   | Managing Git history                  |
| `performance_optimizer` | Performance guidance         | Improving system efficiency           |
| `query_optimizer` | Database query optimization      | SQL optimization                      |
| `release_notes`   | Release documentation            | Version release management            |
| `error_diagnostics` | Systematic error diagnosis     | Troubleshooting failures              |
| `dependency_manager` | Dependency management         | Package/version management            |

---

## 📝 Template Structure

### Tool Template
```xml
<thinking>
[Describe analysis of user's needs]
</thinking>
<prompt_tool>
<tool_name>tool_name</tool_name>
<parameter_type>[parameter_value]</parameter_type>
</prompt_tool>
```

