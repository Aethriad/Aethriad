# 🤝 Contributing Guide

This guide outlines how we work together to keep things clean, consistent, and collaborative. Let's build something stellar. 

---

## ✍️ Commit Style Guide

We follow the [Conventional Commits](https://www.conventionalcommits.org/) standard to keep commit history readable and semantic. This helps us automate changelogs, releases, and makes debugging easier.

| Type       | Purpose                                                      |
|------------|--------------------------------------------------------------|
| `feat`     | New feature                                                  |
| `fix`      | Bug fix                                                      |
| `docs`     | Documentation changes                                        |
| `style`    | Code formatting, white-space, missing semi-colons, etc.     |
| `refactor` | Code change that neither fixes a bug nor adds a feature     |
| `test`     | Adding or updating tests                                     |
| `chore`    | Maintenance, tooling, package updates, etc.                 |
| `perf`     | Performance improvements                                     |

> Example:  
> `feat: add dark mode toggle to header`

---

## 🧱 Naming Conventions

We use consistent naming to keep code readable, scalable, and easy to refactor.

### 🧾 Files & Folders

| Element         | Convention                  | Example                       |
|-----------------|-----------------------------|-------------------------------|
| Folder names     | `kebab-case`                | `user-profile`, `api-utils`   |
| Component files  | `PascalCase`                | `UserCard.tsx`, `Sidebar.tsx` |
| Hooks            | `useCamelCase`              | `useAuth.ts`, `useDarkMode.ts`|
| Utility files    | `camelCase`                 | `formatDate.ts`, `getUser.ts` |
| API routes       | `kebab-case`                | `create-user/route.ts`        |
| Context files    | `PascalCase`                | `AuthContext.tsx`             |

---

## 🌿 Branching Strategy

We follow a simplified GitFlow model to manage changes and releases efficiently:

- `main`: stable production-ready code.
- `dev`: active development branch. All features and fixes are merged here first.
- `feat/*`: feature branches branched from `dev`. Used for new features.
- `fix/*`: fix branches branched from `dev`. Used for bug fixes.
- `hotfix/*`: urgent patches branched from `main`.

> All feature and fix branches should be merged into `dev` via pull requests. Once `dev` is stable and ready for release, it gets merged into `main`.

---

## 📦 Versioning

We use **semantic versioning**: `MAJOR.MINOR.PATCH`

- **MAJOR**: breaking changes (e.g. removed APIs, incompatible logic)
- **MINOR**: new features (e.g. new components, endpoints)
- **PATCH**: bug fixes, performance improvements, small changes

The type of commit defines the impact on the version:

| Commit Type | Version Change |
|-------------|----------------|
| `feat`      | MINOR          |
| `fix`       | PATCH          |
| `perf`      | PATCH          |
| `refactor`  | PATCH (unless breaking) |
| `BREAKING CHANGE` (any type) | MAJOR |

---

By following these guidelines, we ensure our codebase stays healthy, scalable, and accessible for everyone. ✨


