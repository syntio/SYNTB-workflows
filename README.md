# SYNTB-workflows
SYNTB-workflows is a library of reusable workflows centralized for easier maintenance. It contains:

## CI pipeline
This pipeline tests code quality. The yaml file containing the pipeline is located in `.github/workflows/` where all workflows written for GitHub Actions should be placed. The workflow of the pipeline is described in `CI.md` in the root directory.

### SonarCloud
Sonarcloud job in `CI.md` needs an external (not on GitHub) setup. To set up SonarCloud check in your pipeline, you need to:
1. Go to sonarcloud.io
2. Login with your git account
3. Analyze new project
4. Select your project (If you can not find your project, an Admin of your GitHub organization should add your project in settings)

## Dependabot
Dependabot takes the effort out of maintaining your dependencies. You can use it to ensure that your repository automatically keeps up with the latest releases of the packages and applications it depends on. The configuration fle for Dependabot is located in `.github/`. For the full documentation, refer to this [link](https://docs.github.com/en/code-security/supply-chain-security/keeping-your-dependencies-updated-automatically/about-dependabot-version-updates).  
On how to integrate dependabot to your repository, check this [link](https://syntio.atlassian.net/l/c/LEqdbpAF).

## .gitignore
A gitignore file specifies intentionally untracked files that Git should ignore. Files already tracked by Git are not affected. To learn more about gitignore and how it works, refer to [gits documentation](https://git-scm.com/docs/gitignore).

## Code of conduct
In `CODE_OF_CONDUCT.md` is described our standards, what kind of behavior we condone, examples of unaccaptable behavior, the ways community leaders enforce written guidelines, etc.

## License
A permit for anyone to use this project/product as long as they follow the terms and conditions specified in `LICENSE` file.

## Support information
`SUPPORT_INFORMATION.md` holds information on how, where, and when to contact technical support.
