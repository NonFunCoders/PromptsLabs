# 🧠 PromptsLabs  
**AI-Powered Software Development Toolkit**  

A collection of reusable prompt templates to streamline API documentation, architecture design, code refactoring, testing, and more. Built for developers who want to leverage AI effectively while maintaining engineering best practices.

---

## 🚀 Features  
### Core Tools  
| Tool              | Purpose                          | Key Use Case                          |
|-------------------|----------------------------------|---------------------------------------|
| `api_documenter`  | Generate comprehensive API docs  | Missing parameter requirements, authentication, error handling |
| `architecture_advisor` | Evaluate architectural trade-offs | Choosing between Microservices, Monolith, Serverless, etc. |
| `code_refactor`   | Refactor complex code            | Breaking down nested logic, applying design patterns |
| `unit_test`       | Test implementation guidance     | Suggesting testing frameworks/approaches |
| `variable_namer`  | Clean variable naming            | Improving code readability |

### Additional Tools  
- `code_review`: Structured code feedback  
- `commit_assistant`: Commit organization & messages  
- `performance_optimizer`: System performance guidance  
- `query_optimizer`: Database query optimization  
- `release_notes`: Version release documentation  
- `error_diagnostics`: Systematic error diagnosis  
- `dependency_manager`: Package/version management  

<thinking>  
User needs to choose architecture for a data-intensive app.  
</thinking>  
<prompt_tool>  
<tool_name>architecture_advisor</tool_name>  
<options>["Microservices with API Gateway", "Monolith with DDD", "Event-Driven", "Serverless"]</options>  
</prompt_tool>  
<thinking>  
User wants API documentation but missed parameter requirements, authentication, and error responses.  
</thinking>  
<prompt_tool>  
<tool_name>api_documenter</tool_name>  
<auto_followup>  
Include base URL, required/optional parameters with defaults, request examples for JSON/form-data, status codes (200,400,401,403,500), and error response examples.  
</auto_followup>  
</prompt_tool>  
