## How to Use This Template

Follow these steps to set up your custom `src/` template repository and then integrate it into any new Vite project.

### Integrate into a New Vite Project

Whenever you want to start a new Vite project using this custom `src/` template:

1.  **Create a Basic Vite Project:**
    Use `npm create vite@latest` to scaffold a new Vite project. Choose the framework (e.g., React, Vue, Vanilla) that matches your `src/` template.

    ```bash
    npm create vite@latest my-new-project -- --template react-ts # Example for React with TypeScript
    ```

    (Replace `my-new-project` with your desired project name.)

2.  **Navigate into Your New Project:**

    ```bash
    cd my-new-project
    ```

3.  **Remove the Default `src/` Folder:**
    Vite will have created a default `src/` folder. You need to remove this to replace it with your custom one:

    ```bash
    rm -rf src
    ```

4.  **Pull Your Custom `src/` Contents using `degit`:**
    Use the `degit` tool to pull the contents of your template repository directly into the `src/` folder of your new Vite project:

    ```bash
    npx degit your-username/my-custom-src-template src
    ```

    * `npx degit`: Executes `degit` without requiring a global installation.

    * `your-username/my-custom-src-template`: The user/repo name of the Git repository you created in Step 1.

    * `src`: This specifies that the contents of your template repository should be copied into the `src/` directory within your *current* project (`my-new-project`).

5.  **Install Dependencies and Start Development:**
    Finally, install your project's dependencies and start the development server:

    ```bash
    npm install # Or use 'yarn install' or 'pnpm install'
    npm run dev
    ```

You now have a new Vite project initialized with your custom `src/` folder structure, ready for development!
