# 🛠️ Project-Specific Standards Example

*(This file contains example templates. You can copy any standard below, customize it for your project, and paste it into `PROJECT-STANDARDS.md` to force the AI to comply)*

---

## 1. Configuration File Naming Convention (Example)
- **Rule (Required):** All new configuration files must use `kebab-case` and have the `.config.json` suffix.
- **Reason (Required):** Ensures consistency and makes it easy to find configurations across the entire project.
- **Do / Good Example (Optional):** `database-connection.config.json`
- **Don't / Bad Example (Optional):** `DatabaseConnection.json`, `db_config.json`
- **Scope (Optional):** Only applies to configuration files located in the `/config` directory.
- **Exceptions (Optional):** Does not apply to default framework configuration files (e.g., `package.json`, `tsconfig.json`).

## 2. Design System Reusable (Example)
- **Rule (Required):** All UI components (colors, typography, spacing) MUST be inherited from the project's shared Design System (e.g., `theme.ts` or `variables.css`). Absolutely do not hardcode HEX color codes or hard pixels in individual files.
- **Reason (Required):** To easily change the system-wide theme from a single source file.
- **Do / Good Example (Optional):** `color: var(--primary-color);` or `<Button variant="primary" />`
- **Don't / Bad Example (Optional):** `color: #E53935;` or `<button style="background: red;">`

## 3. Shared Logic Directory Management (Example)
- **Rule (Required):** Utility functions (e.g., date format, currency) used 2 or more times must be extracted into Pure Functions and placed in the `src/shared/utils/` directory. Do not write logic directly within UI Components.
- **Reason (Required):** Makes writing Unit Tests easier and adheres to the DRY principle.
- **Do / Good Example (Optional):** `import { formatDate } from '@/shared/utils/date'`
- **Don't / Bad Example (Optional):** Writing date formatting logic directly inside the render logic of a page.
