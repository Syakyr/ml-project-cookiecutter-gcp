# AISG's Cookiecutter Template for End-to-end ML Projects (GCP)

## Table of Contents

- [AISG's Cookiecutter Template for End-to-end ML Projects (GCP)](#aisgs-cookiecutter-template-for-end-to-end-ml-projects-gcp)
  - [Table of Contents](#table-of-contents)
  - [Preface](#preface)
  - [Usage](#usage)
    - [Input Parameters](#input-parameters)
    - [Post-cookiecutter](#post-cookiecutter)
## Preface

This repository contains the
[`cookiecutter`](https://cookiecutter.readthedocs.io/en/stable/)
template for generating a repository that provides boilerplates touching
on the differing components of an end-to-end ML project. This template
is dedicated for the GCP environment.

## Usage

To use the template and create a repository, you would need to
[install the `cookiecutter` CLI](https://cookiecutter.readthedocs.io/en/stable/installation.html)
, say within a virtual environment and pass the URL of this template as
an argument, like such:

```bash
$ pip install cookiecutter
$ cookiecutter https://github.com/aimakerspace/ml-project-cookiecutter-gcp
```

You will then be prompted to provide inputs.These inputs will be used to
populate different parts of the repository to be generated by
`cookiecutter`.

### Input Parameters

|         Parameter        | Detail                                                                                                                                         | Default                                                                     | Choices                                      |
|:------------------------:|------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|----------------------------------------------|
|      `project_name`      | Name of project that will be the header for the `README.md`. Recommended for input to start with alphabet characters. Whitespaces are allowed. | NIL                                                                         | NIL                                          |
|       `description`      | A short description of the project that will be populated in `README.md`.                                                                      | A short description of the project.                                         | NIL                                          |
|        `repo_name`       | Name of the repository folder. Recommended for input to start with alphabet characters. No whitespaces are allowed.                            | `project_name` where whitespaces and underscores are replaced with hyphens. | NIL                                          |
|    `src_package_name`    | Name of the source code's package under `src`. Recommended for input to start with alphabet characters. No whitespaces or hyphens are allowed. | `project_name` where whitespaces are replaced with underscores.             | NIL                                          |
| `src_package_name_short` | The alias for the source code's package.                                                                                                       | `src_package_name`                                                          | NIL                                          |
|     `gcp_project_id`     | ID for the GCP project.                                                                                                                        | NIL                                                                         | NIL                                          |
|       `author_name`      | Your name (or your organisation/company/team). "AISG" is recommended for internal teams.                                                       | NIL                                                                         | NIL                                          |
|   `open_source_license`  | Open source license to be populated within repository. When in doubt, select [3].                                                              | NIL                                                                         | 1 - MIT, 2 - BSD-3-Clause, 3 - No license file |

### Post-cookiecutter

Following the creation of your repository, push the repository to a
remote, and follow its
`README.md` document for a full guide on its usage.
