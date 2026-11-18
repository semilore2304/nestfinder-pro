# NestFinder 🏡

NestFinder is a collaborative real estate web application built by full-stack web development students at Tech Studio Academy.

The project gives students practical experience translating a Figma design into a responsive application using React, TypeScript and Tailwind CSS, while collaborating through Git and GitHub.

Development begins with the frontend. Backend functionality will be introduced in a later phase.

## Project Overview

NestFinder is designed to help users browse properties, view property details and access account features. It also includes an administration area for managing property listings.

This repository contains our class project’s starter structure. Pages, components and functionality will be developed progressively.

## Learning Objectives

By contributing to this project, students will practise:

- Building reusable React components.
- Typing props and application data with TypeScript.
- Creating responsive layouts with Tailwind CSS.
- Implementing navigation with React Router.
- Rendering lists and handling user interactions.
- Managing state and working with forms.
- Organising pages, components, layouts and shared types.
- Collaborating through branches, commits and pull requests.
- Reviewing code and resolving merge conflicts.

## Technology Stack

| Technology | Purpose |
|---|---|
| React | Building the user interface |
| TypeScript | Typing props, data and application logic |
| Vite | Running the development server and building the frontend |
| Tailwind CSS | Styling and responsive layouts |
| React Router | Navigation between pages |
| Git and GitHub | Version control and collaboration |

## Planned Features

### Public Pages

- Homepage.
- Property listings with search and filtering.
- Individual property details.
- Shared navigation and footer.

### Account Pages

- Login.
- Sign up.
- Forgot password.
- Reset password.
- Password reset success.

### Administration Pages

- Dashboard overview.
- Property management.
- Add property.
- Edit property.

### Other Pages

- A 404 page for routes that do not exist.

> During the frontend phase, account and administration screens demonstrate the interface and client-side behaviour. Secure authentication, authorisation and persistent storage will require backend implementation.

## Team Members and Contributions

| Team Member | Assigned Area | Completed Contributions |
|---|---|---|
| Fawaz Jinad | Homepage and shared navigation | To be updated as work is merged |
| Emmanuel Ogunrinde | Property listings | To be updated as work is merged |
| Oreoluwa Onabajo | Property details | To be updated as work is merged |
| Ibrahim Saka | Account pages | To be updated as work is merged |
| Damilola Bakare | Admin area | To be updated as work is merged |

Each team member is responsible for:

- Developing their assigned pages and components.
- Following the supplied Figma design.
- Making layouts responsive and accessible.
- Testing navigation and user interactions.
- Coordinating changes to shared components.
- Submitting work through pull requests.
- Understanding and explaining the code they contribute.

Update the Completed Contributions column when work is reviewed and merged into `main`. Include links to relevant pull requests where possible.

Students may also contribute to testing, bug fixes, shared components and code reviews beyond their assigned areas.

## Project Structure

The React application is located inside the `frontend` folder.

| Location | Contents |
|---|---|
| `frontend/public/` | Static files served directly, including sample JSON data |
| `frontend/src/assets/` | Images, logos and icons imported into components |
| `frontend/src/components/` | Reusable interface components |
| `frontend/src/layouts/` | Shared public and administration layouts |
| `frontend/src/pages/` | Page components connected to routes |
| `frontend/src/services/` | Functions for loading data and making API requests |
| `frontend/src/types/` | Shared TypeScript types and interfaces |
| `frontend/src/App.tsx` | Application composition and routing |
| `frontend/src/main.tsx` | React application entry point |
| `frontend/src/index.css` | Global styles and the Tailwind CSS import |

Additional folders may be introduced as development progresses.

## Getting Started

### 1. Check Your Tools

You will need:

- A supported Node.js LTS version compatible with the project.
- npm.
- Git.
- A GitHub account.
- A code editor such as Visual Studio Code.

Check your installed versions:

```bash
node --version
npm --version
git --version
```

### 2. Clone the Repository

On this repository’s GitHub page:

1. Click **Code**.
2. Select **HTTPS**.
3. Copy the repository URL.
4. Open your terminal in the folder where you keep your projects.
5. Replace `REPOSITORY_URL` below with the copied URL and run:

```bash
git clone REPOSITORY_URL
```

Clone the repository once. You do not need to clone it before every class.

### 3. Enter the Frontend Folder

From the folder containing the cloned repository, run:

```bash
cd nestfinder
cd frontend
```

If the cloned folder has a different name, use that name instead of `nestfinder`.

### 4. Install Dependencies

Inside `frontend`, run:

```bash
npm install
```

This installs the packages listed in `package.json`.

### 5. Start the Development Server

```bash
npm run dev
```

Open the local URL displayed in the terminal.

Keep the terminal running while you work. To stop the server, press **Ctrl + C**.

## Returning to the Project

When starting another development session:

1. Open the project in your editor.
2. Open a terminal.
3. Check your terminal’s current folder.
4. Navigate into `frontend` if necessary.
5. Start the development server:

```bash
npm run dev
```

If your terminal is already inside `frontend`, do not run `cd frontend` again.

Run `npm install` again when dependencies have changed or the `node_modules` folder is missing.

## Team Collaboration Workflow

Work on a separate branch for your assigned feature.

### 1. Check Your Current Work

```bash
git status
```

Commit your current work before switching branches. Ask your instructor for guidance if you are unsure how to handle unfinished changes.

### 2. Update Your Local Main Branch

```bash
git switch main
git pull origin main
```

This brings the latest shared changes into your local `main` branch.

### 3. Create a Feature Branch

Choose a short name describing your task:

```bash
git switch -c feature/property-listings
```

Suggested branch names include:

| Assigned Area | Example Branch |
|---|---|
| Homepage and shared navigation | `feature/homepage-navigation` |
| Property listings | `feature/property-listings` |
| Property details | `feature/property-details` |
| Account pages | `feature/account-pages` |
| Admin area | `feature/admin-area` |

Create a branch once. To return to an existing branch, use:

```bash
git switch feature/property-listings
```

Replace the example with your branch name.

### 4. Complete Your Assigned Work

- Follow the supplied Figma design.
- Use reusable components where appropriate.
- Check desktop and mobile layouts.
- Test links, buttons, forms and other interactions.
- Check the browser console for errors.

Coordinate with your instructor and teammates before changing shared routing, layouts, configuration or dependencies.

### 5. Review and Commit Your Changes

Check what changed:

```bash
git status
git diff
```

Stage the relevant files using their actual paths. For example, from the repository root:

```bash
git add frontend/src/pages/PropertyPage.tsx
```

If your task changes several files, stage each relevant file.

Commit with a clear message:

```bash
git commit -m "Build responsive property listings page"
```

Other examples:

```text
Add homepage hero section
Create property details layout
Build responsive login form
Fix mobile navigation spacing
Add admin property table
```

### 6. Push Your Branch

```bash
git push -u origin feature/property-listings
```

Use your own branch name.

After the upstream connection is established, later pushes from that branch can use:

```bash
git push
```

### 7. Open a Pull Request

On GitHub:

1. Open the repository.
2. Select **Compare & pull request**.
3. Set the base branch to `main`.
4. Confirm that the comparison branch is your feature branch.
5. Add a clear title and description.
6. Include screenshots for interface changes.
7. Submit the pull request for review.

Explain:

- What you built or changed.
- How you tested it.
- Any incomplete work or known issues.

Wait for review before merging. Do not push directly to `main` unless your instructor asks you to.

## Updating an Existing Feature Branch

First, commit your current changes. Then run:

```bash
git switch main
git pull origin main
git switch feature/property-listings
git merge main
```

Replace `feature/property-listings` with your branch name.

This brings the latest local `main` changes into your feature branch.

If Git reports merge conflicts:

1. Open the affected files.
2. Review both versions.
3. Keep or combine the correct changes.
4. Remove the conflict markers.
5. Save and stage the resolved files.
6. Complete the merge commit.
7. Test the application again.

Ask your instructor for support if you are unsure which changes to keep.

## Coding Guidelines

### Components and Files

- Use PascalCase for component names, such as `PropertyCard`.
- Match component filenames to their names, such as `PropertyCard.tsx`.
- Use `.tsx` for files containing JSX.
- Use `.ts` for types and utility functions without JSX.
- Match import paths to the exact filename casing.

### TypeScript

- Define clear types for component props and shared data.
- Use `import type` when importing types.
- Avoid `any` when a specific type is available.
- Resolve TypeScript errors before submitting work.

Example:

```tsx
import type { Property } from "../types/Property";
```

### List Rendering

Use stable, unique keys when rendering lists:

```tsx
{properties.map((property) => (
  <PropertyCard
    key={property.id}
    property={property}
  />
))}
```

Every property in the list must have a unique `id`.

### Styling and Accessibility

- Follow the supplied design.
- Use responsive Tailwind CSS classes.
- Add meaningful alternative text to informative images.
- Associate form inputs with labels.
- Use buttons for actions and links for navigation.
- Provide visible keyboard focus styles.

### Dependencies and Generated Files

- Discuss new packages with your instructor before installing them.
- Commit `package-lock.json` when an intentional dependency change updates it.
- Do not commit `node_modules`, build output or secret credentials.

## Before Opening a Pull Request

- [ ] My assigned feature works.
- [ ] The layout works on mobile and desktop.
- [ ] Links and buttons behave as expected.
- [ ] Form inputs have appropriate labels.
- [ ] There are no unexplained browser console errors.
- [ ] Rendered lists use unique keys.
- [ ] I have removed unused imports and temporary debugging code.
- [ ] The production build passes.
- [ ] My commit messages describe my changes.
- [ ] My pull request includes screenshots where useful.

From `frontend`, check the production build:

```bash
npm run build
```

If the project includes a lint script, also run:

```bash
npm run lint
```

## Common Problems

| Problem | What to Check |
|---|---|
| npm cannot find `package.json` | Make sure your terminal is inside `frontend` |
| A package cannot be found | Run `npm install` inside `frontend` |
| An import cannot be resolved | Check the path, spelling and filename casing |
| React reports duplicate keys | Give every item in the rendered list a unique ID |
| Changes appear to be missing | Confirm the file is saved and the correct branch is checked out |
| A merge conflict appears | Review and resolve the conflicting changes |
| The server uses another port | Open the URL printed in the terminal |
| Unexpected files are staged | Run `git status` and review the staged changes |

When asking for help, share the exact error message, the relevant code and the command you ran.

## Project Development Phases

| Phase | Focus |
|---|---|
| 1 | Repository setup and shared frontend structure |
| 2 | Responsive pages and reusable components |
| 3 | Routing, forms and client-side interactions |
| 4 | Integration, testing and interface improvements |
| 5 | Backend development and API integration |

## Credits

**Institution:** Tech Studio Academy  
**Instructor:** Bukola Ruth Olafenwa  
**Project:** NestFinder  
**Design reference:** Class-provided Figma design

### Student Contributors

- Fawaz Jinad
- Emmanuel Ogunrinde
- Oreoluwa Onabajo
- Ibrahim Saka
- Damilola Bakare

Build thoughtfully, communicate with your teammates and commit your progress regularly.