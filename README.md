# GitHub Actions workflow template for LaTeX document compilation (minimal)

This is a template for authors using LaTeX to use GitHub Actions based workflows to compile their documents.

The latest output file can be found: [mydocument.pdf on branch pdf-output](../pdf-output/mydocument.pdf)

This work was presented in a workshop at [TUG 2024](https://www.tug.org/tug2024/) and a corresponding article was published in [TUGboat 140](https://tug.org/l/peischl-cicd2024).
The linked repository includes a list of all variants of CI templates provided like this one.

## Usage

To use this for your own documents, you can either create a new repository based on this template or copy the workflow configuration (`.github/`) into your own project.

This variant is using a minimal TeX Live setup based on a file listing the dependencies.
This saves disk space on the server running the build and may be faster for an individual run.

In case you load additional packages please be aware that you have to include those into `.github/tl_packages`.
We recommend using the [Island of TeX's Dependency Printer](https://gitlab.com/islandoftex/texmf/depp) for this purpose.

If you compile lots of different documents this may increase the maintenance effort and therefore it might be more useful to take a look at the [Workflow Template using a full TeX Live installation](../../../github-actions-latex).

## LICENSE

We want this to be used. You can find all this within the documentation. But in case you care, this work is licensed under MIT License.
