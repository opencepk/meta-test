![cepk-template-base-logo](assets/project-logo.png)

# cepk-template-base

CEPK Cloud Engineering Platform Kit - Template Base - Base git project template containing README, pre-commit and ghactions workflows

----

Welcome to the `CEPK Cloud Engineering Platform Kit - Template Base - HOWTO`

This project is a base template github repo that can be used in any code project.
It can also be used (forked) as the base for other CEPK Cloud Engineering Platform Kit github repo templates.

## What's here

<!--TOC-->

- [cepk-template-base](#cepk-template-base)
  - [What's here](#whats-here)
  - [Creating a project from this template](#creating-a-project-from-this-template)
  - [Seed the new project with .project.properties.json](#seed-the-new-project-with-projectpropertiesjson)
  - [Contributing](#contributing)

<!--TOC-->

## Creating a project from this template

* 1 - When creating a new github repository - select this project `opencepk/cepk-template-base` in the `Repository template` field as shown below:

![template-howto-create-repo-from-template.png](assets/template-howto-create-repo-from-template.png)

## Seed the new project with .project.properties.json

* 1 - Now that your project was generated from the template, clone it to your local machine.

* 2 - Edit the file `.project-properties.json.template` and update the values to match the values for your new code project.

* 3 - Rename the file `.project-properties.json.template` to `.project-properties.json`

* 4 - Run `pre-commit run -a` on the project to replace the template values in this template project with the values in `.project-properties.json`

> NOTE: When pre-commit updates files, it will fail on the steps that updated files - this is expected so run `pre-commit run -a` again to ensure everything is clean.

* 5 - Continue to build and develop your project as needed.

## Contributing

If you notice any issues, concerns of possible improvements, please make a branch and pull request on this project.
Or if you prefer get in touch with the @opencepk/tcx-platform-devops team.


When developing against this project - run the following command to ensure pre-commit hooks run successfully.

> NOTE: This project is designed for the `find-and-replace-strings` pre-commit hook to only run on code projects created from this template.

```bash
source .pre-commit-template-skip-hooks.sh
```
