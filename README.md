# GitHub Workflows Repository

This repository serves as the central hub for shared GitHub Actions workflows and actions, enabling consistent CI/CD practices and automation efficiencies across all projects within our organization.

## Getting Started

To utilize these workflows and actions in your project, follow the steps below:

1. **Browse the Repository**: Look through the available workflows in the `workflows` directory to find one that suits your project's needs.
2. **Reference the Workflow**: In your project's `.github/workflows` directory, create a new workflow file (e.g., `main.yml`). Use the `uses` keyword to reference the shared workflow from this repository. For example:

    ```yaml
    name: CI
    on: [push]
    
    jobs:
        build:
        uses: our-org/github-workflows/.github/workflows/build.yml@main
    ```

3. **Customize Parameters**: Some workflows may allow for customization through input parameters. Make sure to review the workflow's documentation and adjust any necessary parameters in your project's workflow file.

## License

This project is licensed under the MIT License. See [LICENSE.md](LICENSE.md) for details.