# Setting Up Cursor AI with Rules and Vibe Coder 🚀

This guide explains how to set up Cursor AI with custom rules and use Vibe Coder for generating detailed requirement specifications.

## Setting Up Cursor AI Rules ⚙️

1. **Open Cursor IDE**
2. **Go to Settings (⚙️)**
3. **Navigate to Rules section**
4. **Click on Create New Rule**
5. **Name your rule** appropriately based on the stack/purpose
6. **Copy and paste** the relevant rule configuration

### Creating Custom Rules for Your Project 🛠️

You are **not limited** to the predefined rules. If your project has specific requirements—such as **custom component systems** in `src/components`—feel free to **create new rules** reflecting those details. For instance, if you already have common components like **Button, Table, Menu, Card, etc.**:

- Make sure your **new rules** inform Cursor about the existing components.
- **Before writing any new code**, verify whether a similar component already exists in `src/components`.
- **Update existing components** if necessary, rather than duplicating them.

### Available Stack-Specific Rules 🌐

Below are various technology stacks and their corresponding rules:

#### Next.js

- **Stack**: Next.js 15, Tailwind CSS
- **Key Features**:
  - App Router-based routing
  - Server Components by default
  - TypeScript support
  - Tailwind CSS styling
  - API routes in `src/app/(home)` directory

#### React

- **Stack**: React 19, Tailwind CSS
- **Key Features**:
  - React Router DOM for navigation
  - TypeScript support
  - External REST API integration
  - Environment-specific API configurations

#### React Native

- **Stack**: React Native, CSS/NativeWind
- **Key Features**:
  - React Navigation
  - TypeScript support
  - CSS Stylesheet or NativeWind for styling
  - External REST API integration

#### Expo

- **Stack**: Expo, NativeWind
- **Key Features**:
  - Expo Router for navigation
  - NativeWind and CSS stylesheet for styling
  - External REST API integration
  - Environment-specific configurations

#### Django

- **Stack**: Django, Django REST Framework
- **Key Features**:
  - Django REST Framework for API development
  - Django Admin for admin panel
  - APIs built in `api/v1/(appname)` directory
  - Built-in authentication and security features

## Using Vibe Coder for Requirements 💡

To generate detailed requirement specifications using **Vibe Coder**:

1. **Open Cursor's Command Palette**
   - `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (Mac)
2. **Search for "Composer"** and open it
3. **Access Vibe Coder** at: [Vibe Coder GPT](https://chatgpt.com/g/g-67cd2d36e07c8191944db1b88f629f4c-vibe-coder)

### Writing Effective Requirements ✍️

When writing requirements in Vibe Coder, include:

1. **API Endpoints**: Provide complete API URLs
2. **Request Format**: Include any FormData or request body structure
3. **Response Format**: Add example API responses
4. **Visual References**: Attach relevant images/mockups
5. **Business Logic**: Clearly state any business rules or conditions

### Example Requirement Specification 📄

```yaml
Feature: Post Reports Management Dashboard

Overview:
- Admin panel built with Next.js 15 and Tailwind CSS
- Custom component library in src/components
- Page for handling post reports with overview cards and tabbed tables

API Endpoints:
1. Dashboard Overview:
   - URL: https://developers-learn.talrop.com/api/v1/posts/reports-dashboard/
   - Method: GET
   - Response: {
       "status_code": 6000,
       "data": {
           "total_reports": 557,
           "post_reports": 556,
           "comment_reports": 1,
           "pending_evaluvations": 5,
           "distant_post_report": 4,
           "distant_comments_report": 1
       }
   }

2. Post Reports List:
   - URL: https://developers-learn.talrop.com/api/v1/posts/list-reports/?report_type=posts
   - Method: GET
   - Parameters: report_type (posts/comments)

UI Components:
1. Overview Cards showing:
   - Total Reports
   - Post Reports
   - Comment Reports
   - Pending Evaluations

2. Tabbed Table Interface:
   - Tabs: Posts / Comments
   - Columns:
     - Post Info
     - Author Info
     - Number of Reports
     - Evaluation Status
     - Actions
```

## Best Practices ⭐

1. **Always name rules** according to their specific use case or stack
2. **Include complete API documentation** in requirements
3. **Provide example responses** for better context
4. **Attach UI mockups** when available
5. **Specify any dependencies** or custom components being used

## Common Coding Preferences Across Stacks 🏗️

1. **Code Organization**

   - Keep solutions simple and maintainable
   - Avoid code duplication
   - Keep files under 200-300 lines
   - Maintain a clean and organized codebase

2. **Environment Handling**

   - Write code considering dev, test, and prod environments
   - Never overwrite .env files without confirmation
   - Use environment-specific configurations

3. **Testing and Data**

   - Write thorough tests for major functionality
   - Use mocking only for tests, never for dev/prod
   - Avoid stubbing or fake data in production code

4. **Change Management**
   - Focus on task-relevant code areas
   - Avoid unnecessary pattern/architecture changes
   - Consider impact on related code areas
   - Make only well-understood changes

---

## Next Steps: Composing Requirements in Cursor 📝

After generating your **requirements in Vibe Coder**, the next step is to **copy and paste** the requirement specification into the **Cursor Composer**.

1. **Add Context with the Rules**

   - Before you paste your requirements, **provide the relevant context** by referencing the **stack-specific rules** you intend to use.
   - If you have any images, wireframes, or design files, attach them or refer to them so that **Cursor** can fully understand how to structure your components.

2. **Paste the Requirements**

   - Copy your **API, request/response format, and business logic** details directly into the Composer.
   - Include any **important clarifications** or instructions not covered in the initial rule set.

3. **Instruct Cursor to Generate the Components**
   - Clearly state which components, pages, or features you need built.
   - Remind Cursor about the relevant best practices and guidelines you’ve established.

### Important Note ⚠️

**Cursor AI** is **not** a complete replacement for a developer’s work. It is meant to **augment** your efficiency. Always:

- **Review every line of code** written by Cursor for quality and security.
- Remember that **all responsibility** for the generated code is ultimately yours.
- Accept code only if it meets your **standards** and **requirements**.

---

**Happy Building!** 🎉  
Keep your code organized, secure, and well-documented. By following these steps, you’ll help ensure your Cursor AI experience remains efficient, productive, and aligned with your project goals.
