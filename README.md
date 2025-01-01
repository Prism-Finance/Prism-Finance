# Prism Finance - Monorepo

This is a monorepo containing the backend and frontend components of the Prism Finance application, managed as Git submodules.

## Structure

```
prism-finance/
├── backend/           # Backend API and services (submodule)
├── frontend-mobile/   # Mobile frontend application (submodule)
├── frontend-web/      # Web frontend application (submodule)
├── docs/              # Documentation
├── deployment/        # Deployment configurations
```

## Getting Started

1. Clone the repository with submodules:
   ```bash
   git clone --recurse-submodules https://github.com/Prism-Finance/Prism-Finance.git
   ```
2. Initialize and update submodules:
   ```bash
   git submodule update --init --recursive
   ```
3. Install dependencies in each submodule:
   ```bash
   cd backend && bun install
   cd ../frontend-mobile && bun install
   cd ../frontend-web && bun install
   ```

## Submodules

- [backend](https://github.com/Prism-Finance/backend): Backend API and services
- [frontend-mobile](https://github.com/Prism-Finance/frontend-mobile): Mobile frontend application
- [frontend-web](https://github.com/Prism-Finance/frontend-web): Web frontend application

## Development

To work with submodules:

- Update all submodules to latest:
  ```bash
  git submodule update --remote
  ```
- Commit changes in submodules:
  ```bash
  git add backend frontend-mobile frontend-web
  git commit -m "Update submodules"
  ```

## Contributing

Please see [CONTRIBUTING.md](docs/development/CONTRIBUTING.md) for contribution guidelines.
