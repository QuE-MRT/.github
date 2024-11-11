![QuE_Logo_cropped](https://user-images.githubusercontent.com/18266223/200273741-876ecea9-f357-4362-86be-5b38e9338ffc.png)

# QuE-MRT GitHub

Welcome to the QuE-MRT GitHub organization! This README provides essential guidelines for cloning repositories, setting up your environment, and following best practices for collaborative development.

The QuE-MRT project aims to build a commercially available end-to-end platform to enhance, acquire and visualize magnetic resonance signals of metabolic processes in humans by use of [Hyperpolarization](https://en.wikipedia.org/wiki/Hyperpolarization_(physics)). The goal is to translate Hyperpolarized (HP) Magnetic Resonance Imaging (MRI) into clinical applications in Germany and worldwide. The project is funded by the German agency Bundesministerium für Bildung und Forschung (BMBF) for four years (2022 - 2026) and brings together three German universities and four companies. Read more about QuE-MRT [here](https://www.quantentechnologien.de/forschung/foerderung/leuchtturmprojekte-der-quantenbasierten-messtechnik/que-mrt.html).

---

## Table of Contents

- [Cloning Repositories](#cloning-repositories)
- [Setting Up Your Environment](#setting-up-your-environment)
- [Branching Strategy](#branching-strategy)
- [Commits and Pull Requests](#commits-and-pull-requests)
- [Coding Standards](#coding-standards)
- [Code Review Process](#code-review-process)
- [Contact and Support](#contact-and-support)

---

## Cloning Repositories

To clone a repository from this organization:

1. Navigate to the repository you wish to clone on GitHub.
2. Click the "Code" button and copy the repository URL (either SSH or HTTPS).
3. Open your terminal, navigate to the directory where you want to store the repository, and enter:

    ```bash
    git clone <repository_url>
    ```

Replace `<repository_url>` with the copied URL of the repository.

> **Note**: Ensure you have the proper permissions to clone and contribute to repositories in this organization.

---

## Setting Up Your Environment

1. Make sure you have [Git](https://git-scm.com/downloads) installed on your local machine.
2. If using SSH, configure your SSH keys with GitHub by following [these instructions](https://docs.github.com/en/authentication/connecting-to-github-with-ssh).
3. Follow any specific repository setup instructions in its `README.md` file.

---

## Branching Strategy

To maintain an organized Git history, please adhere to the following branching strategy:

1. **Main Branch**: The production-ready branch. Only tested and approved changes should be merged here.
2. **Development Branch**: All new features and bug fixes should start here before going to `main`.
3. **Feature/Hotfix Branches**: Create new branches for each feature or hotfix. Name these as follows:
   - Features: `feature/feature-name`
   - Hotfixes: `hotfix/issue-description`

Example:

```bash
git checkout -b feature/add-new-feature
```

---
 
## Commits and Pull Requests

1. Write clear, descriptive commit messages that explain the purpose of the change.
2. Open a Pull Request (PR) when your work is ready for review. Be sure to:
   - Set the correct base branch for your PR (usually development).
   - Provide a summary of the changes and link any relevant issues.
   - Request at least one reviewer from the team.
  
---

## Coding Standards
To ensure consistency across our codebase, please follow these standards:

- Code Formatting: Adhere to the language-specific formatting rules (e.g., [Prettier](https://prettier.io/) for JavaScript, [Black](https://pypi.org/project/black/) for Python, [Style Guidelines](https://de.mathworks.com/matlabcentral/fileexchange/45047-matlab-style-guidelines-cheat-sheet) for Matlab).
- Documentation: Document functions, classes, and modules as needed.
- Testing: Ensure your code includes appropriate tests and passes all existing tests before making a pull request.

---

## Code Review Process
1. Reviewers should check for code quality, adherence to standards, and the absence of bugs.
2. Once the PR is approved by at least one reviewer, you may merge it into the development branch.
3. After merging, update your local development branch and delete the feature/hotfix branch (both locally and remotely if needed):
   ´´´bash
   git checkout development
   git pull origin development
   git branch -d <branch-name>
   git push origin --delete <branch-name>
   ´´´

---

## Licensing for Open-Source Contributions

For any open-source repositories in this organization, contributors are encouraged to use either the **MIT License** or the **GNU General Public License v3 (GPLv3)** to ensure that projects remain accessible and freely usable by the community. 

### Choosing a License

- **MIT License**: A permissive license that allows for minimal restrictions on reuse, making it ideal for projects where you want to maximize compatibility and ease of integration with other projects. 
- **GPLv3**: A copyleft license that requires derivative works to remain open-source and licensed under GPLv3, ensuring the project's continued openness even as it’s modified and distributed by others.

### Adding a License to Your Repository

1. **Create a `LICENSE` file** at the root of your repository.
2. Select your preferred license template:
   - For MIT, use [this MIT License template](https://choosealicense.com/licenses/mit/).
   - For GPLv3, use [this GPLv3 template](https://choosealicense.com/licenses/gpl-3.0/).
3. Paste the license text into the `LICENSE` file and fill in any required information, such as the year and your name.
4. Commit the `LICENSE` file to your repository.

> **Note**: Please consult with your project lead or organization admins if you are unsure about which license to use.

---

## Contact and Support

For questions, discussions, or support, please reach out to one of the organization admins.




