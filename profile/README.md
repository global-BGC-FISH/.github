# Description and guideline on the global-BGC-FISH organization
![VOICES logo](../VOICES_logo.png)

## What is the global-BGC-FISH organization?
This organization hosts repositories and software tools developed in support of the global-BGC-FISH initiative. It brings together projects focused on marine biogeochemistry, ecosystem dynamics, fisheries research, and data-driven analyses relevant to global ocean processes. The repositories in this organization aim to provide reproducible workflows, model outputs, and analysis tools for scientific investigation and collaborative development.

## Guideline for a repository in the organization

### How to add a repository?
Requirements to add a repository to the organization [https://github.com/global-BGC-FISH]:
- Be a member of the [global-BGC-FISH](https://github.com/global-BGC-FISH) organization or have a documented collaboration scope.
- Put the mandatory files in the repository as described [here](#content-of-a-repository).
- Follow the [recommendations](#recommendations) as much as possible.
- Complete the table below with the relevant repository information.

| Repository name | Responsible[^1] | Theme | Short description |
| :---: | :---: | :---: | :--- |
| [.github](https://github.com/global-BGC-FISH) | [@plazzari](https://github.com/plazzari) | Organization | Organization profile and default repository configuration |


[^1]: Indicate here the GitHub login of the main contact(s) for the code.

### Content of a repository
A GitHub repository of the global-BGC-FISH organization should contain the following files:

- A `LICENSE` file: open-source licensing is encouraged.
- A `CODEOWNERS` file: indicate the main contacts for the repository. See [here](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners) for more details.
- A `README` file: see the minimum requirement for the README file [here](#readme).
- One or several notebooks or reproducible examples to demonstrate the workflow with a standard application.

#### README
The README file should include a description of:
- the scientific or data source used
- the baseline method or a link to the relevant notebook or workflow
- the validation metrics used, when applicable
- the list of dependencies and their versions, with language-specific installation instructions when relevant
- the documentation and references needed for reuse and understanding of the code
- any relevant citations or links to publications connected to the project

### Recommendations
In addition to the points mentioned above, it is strongly suggested to:
- Use data APIs or versioned datasets when available to make testing and reproducibility easier.
- For complex projects, use GitHub Actions to run tests when pushing to the repository or merging changes into the `main` branch. See [here](https://docs.github.com/en/actions) for documentation.
- Use language-specific environment tools such as `conda`, `pipenv`, or a container configuration when appropriate.
- Follow current best coding practices and maintain readable, modular, documented code.
- Keep code specific to the global-BGC-FISH scope in this organization; more general-purpose tools may be hosted elsewhere.

