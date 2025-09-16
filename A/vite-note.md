# To Create Vite project

Let's create a Vite project step-by-step using Markdown. Vite is a modern frontend build tool that significantly improves the developer experience with its lightning-fast cold server start and instant Hot Module Replacement (HMR).

## Creating a Vite Project

This guide will walk you through creating a new Vite project using npm (Node Package Manager).

### Prerequisites

Before you begin, ensure you have Node.js installed on your system. You can download it from [nodejs.org](https://nodejs.org/). It's recommended to use an LTS (Long Term Support) version.

### Step 1: Open Your Terminal or Command Prompt

Navigate to the directory where you want to create your new project using your terminal or command prompt.

### Step 2: Run the Vite Create Command

Execute the following command in your terminal. This command will prompt you to enter your project name and select a framework.

```bash
npm create vite@latest
```

### Step 3: Enter Your Project Name

The command will first ask for your project name. Enter a name for your project (e.g., `my-vite-app`) and press Enter.

```
✔ Project name: … my-vite-app
```

### Step 4: Select a Framework

Next, you'll be presented with a list of frameworks. Use the arrow keys to select your preferred framework. For this example, we'll select `React`.

```
✔ Select a framework: › React ▮ Vue ▮ Preact ▮ Lit ▮ Svelte ▮ Solid ▮ Qwik ▮ Astro
```

### Step 5: Select a Variant (Optional)

After selecting a framework, you might be prompted to choose a variant. For React, you can typically choose between `React` (with JavaScript) and `React + SWC` (with TypeScript and SWC for faster compilation). Let's choose `React` for simplicity.

```
✔ Select a variant: › React ▮ React + SWC
```

### Step 6: Navigate into Your Project Directory

Once the scaffolding is complete, change into your newly created project directory.

```bash
cd my-vite-app
```

### Step 7: Install Dependencies

Install the necessary project dependencies using npm.

```bash
npm install
```

### Step 8: Run the Development Server

Start the Vite development server. This will launch your application in your browser, usually at `http://localhost:5173/`.

```bash
npm run dev
```

### Step 9: View Your Application

Open your web browser and navigate to the URL provided by the `npm run dev` command (e.g., `http://localhost:5173/`). You should see the default Vite starter page for your chosen framework.

### Project Structure (Example for React)

After creating the project, your directory structure will look something like this:

```
my-vite-app/
├── public/
│   └── vite.svg
├── src/
│   ├── assets/
│   │   └── react.svg
│   ├── App.css
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
├── .gitignore
├── index.html
├── package.json
├── README.md
├── vite.config.js
└── ... (other config files)
```

### Next Steps

*   **Explore the Code:** Open the `src` folder and start modifying the `App.jsx` (or equivalent for your chosen framework) and `index.css` files to build your application.
*   **Build for Production:** When you're ready to deploy, run `npm run build` to create an optimized production build in the `dist` folder.
*   **Configuration:** You can customize Vite's behavior by editing the `vite.config.js` file.

Congratulations! You have successfully created a Vite project and are ready to start developing.