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

4.  **Unzip Your Custom `src/` Contents:**
    Copy your zipped `src` template file into your new project's root directory, then unzip it directly into the `src/` folder.

    ```bash
    # Example using `unzip` command (you might need to install this if not available)
    cp /path/to/src.zip . # Copy the zip file to the current directory
    unzip src.zip -d src/  # Unzip it into the 'src' folder
    rm src.zip             # (Optional) Remove the zip file after extraction
    ```
    Alternatively, you can manually extract the contents of your `src` template zip file into the `src/` folder of your new project using your operating system's file explorer.

    **Note:** You will need to manually manage the creation and distribution of your `src` template as a `.zip` file.
      

5.  **Install Dependencies and Start Development:**
    Finally, install your project's dependencies and start the development server:

    ```bash
    npm install # Or use 'yarn install' or 'pnpm install'
    npm run dev
    ```

You now have a new Vite project initialized with your custom `src/` folder structure, ready for development!
