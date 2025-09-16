
## Creating a New Next.js Project

This guide will walk you through the process of creating a new Next.js project from scratch.

### Prerequisites

*   **Node.js:** Ensure you have Node.js installed on your system. You can download it from [nodejs.org](https://nodejs.org/). It's recommended to use a recent LTS version.
*   **npm or Yarn:** These are package managers that come with Node.js or can be installed separately. We'll use `npx` (which comes with npm 5.2+) for this guide, as it allows you to run Node.js package executables without globally installing them.

### Step 1: Open Your Terminal or Command Prompt

Navigate to the directory where you want to create your new project. You can use the `cd` command for this.

```bash
# Example: Navigate to your projects folder
cd ~/Projects
```

### Step 2: Create a New Next.js App

We'll use the `create-next-app` command-line tool to set up your project. This tool will guide you through some basic configuration options.

Run the following command, replacing `my-nextjs-app` with your desired project name:

```bash
npx create-next-app@latest my-nextjs-app
```

You will be prompted with a series of questions:

1.  **Would you like to use TypeScript?** (Recommended)
    *   Type `y` and press Enter for TypeScript, or `n` for JavaScript.
2.  **Would you like to use ESLint?** (Recommended)
    *   Type `y` and press Enter to enable ESLint for code linting.
3.  **Would you like to use Tailwind CSS?** (Recommended)
    *   Type `y` and press Enter to include Tailwind CSS for styling.
4.  **Would you like to use `src/` directory?**
    *   Type `y` to organize your code within a `src/` folder, or `n` for a flat structure.
5.  **Would you like to use App Router? (recommended)**
    *   Type `y` to use the newer App Router (recommended for new projects), or `n` to use the older Pages Router.
6.  **Would you like to customize the default import alias?**
    *   Type `y` if you want to customize the alias (e.g., `@/*`), or `n` to use the default (`@/*` with App Router, `~/*` with Pages Router).

The tool will then download the necessary packages and set up your project structure.

### Step 3: Navigate into Your Project Directory

Once the installation is complete, change your current directory to the newly created project folder:

```bash
cd my-nextjs-app
```

### Step 4: Run the Development Server

Now, you can start the development server to see your new Next.js application in action.

```bash
npm run dev
# or
yarn dev
```

This command will start a local development server, usually at `http://localhost:3000`.

### Step 5: View Your Application

Open your web browser and go to `http://localhost:3000`. You should see the default Next.js welcome page.

### Project Structure (with App Router and `src/` directory)

After running `create-next-app` with the recommended options (TypeScript, ESLint, Tailwind, `src/`, App Router), your project structure will look something like this:

```
my-nextjs-app/
├── public/             # Static assets like images, fonts
├── src/
│   ├── app/            # App Router directory
│   │   ├── favicon.ico
│   │   ├── globals.css # Global styles
│   │   ├── layout.tsx  # Root layout component
│   │   └── page.tsx    # The root page component (index page)
│   └── ...             # Other source files (components, utils, etc.)
├── .eslintrc.json      # ESLint configuration
├── .gitignore          # Files to ignore in Git
├── next.config.js      # Next.js configuration
├── package.json        # Project dependencies and scripts
├── postcss.config.js   # PostCSS configuration (for Tailwind CSS)
├── README.md           # Project README
├── tailwind.config.ts  # Tailwind CSS configuration
└── tsconfig.json       # TypeScript configuration
```

### Next Steps

Congratulations! You've successfully created a new Next.js project. You can now start building your application by:

*   **Editing `src/app/page.tsx`**: This is the main page component for your application's homepage.
*   **Creating new routes**: Add new folders inside `src/app/` to create new pages. For example, `src/app/about/page.tsx` will create a route at `/about`.
*   **Adding components**: Create reusable components within the `src/` directory.
*   **Styling**: Use Tailwind CSS classes or global CSS to style your application.

Happy coding!