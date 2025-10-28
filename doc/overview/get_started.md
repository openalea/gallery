# Get Started

## Organization

Tutorials are approximately divided first into thematical scientific sections, focusing onto use of individual packages, then into a more integrated view mixing different topics and openalea packages.

Most of the tutorial content is written as Jupyter Notebooks that mixes code, text, visualization, and exercises. You can either browse rendered versions of these notebooks on this website, or _execute_ the code examples interactively.

You can execute code examples either on the Cloud  or on your computer with minimal setup.
## Run code interactively

### On the Cloud

The easiest way to start modifying and experimenting with tutorial content is to launch a pre-configured server on the Cloud. This is easy thanks to several free resources which offer ephemeral computing instances (be aware you may loose your connection or work at any time)

```{warning}
Be patient, it can take a few minutes for a server to become available on the Cloud!
```

#### Mybinder.org

Clicking [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/openalea/gallery/release2025) will load a pre-configured Jupyter Lab interface with _all_ tutorial notebooks for you to run. _You have minimal computing resources and any changes you make will not be saved._ Any page with executable content also has a 🚀 icon in the upper right that will launch an interactive session for that particular page.

#### GitHub Codespaces

This tutorial is available to run within [GitHub Codespaces](https://github.com/features/codespaces) - a preconfigured development environment running in Microsoft Azure.

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new/openalea/gallery)

☝️ Click the button above to go to options window to launch a GitHub codespace.

You can choose from a selection of virtual machine types: 2 cores - 8 GB RAM should be sufficient for all code examples in this repository.
Additionally, you are able to chose from various configurations for specific workshops (such as Scipy2024).
GitHub currently gives every user [120 vCPU hours per month for free](https://docs.github.com/en/billing/managing-billing-for-github-codespaces/about-billing-for-github-codespaces#monthly-included-storage-and-core-hours-for-personal-accounts), beyond that you must pay. **So be sure to explicitly stop your codespace when you are done by going to this page (https://github.com/codespaces).** You can also chose to fully delete your codespace when you're done exploring tutorial content.

```{tip}
By default Codespaces open VSCode in a browser window. But you can also launch a JupyterLab interface. Once you've launched a codespace, use the auto-generated name in the following URL: `https://github.com/codespaces/CODESPACE-NAME?editor=jupyter`
```

Using the GitHub CLI is another very convenient way to start a codespace:

```bash
gh codespace create -R openalea/gallery
```

```bash
# Wait a few minutes for `gh codespace create` to finish, then run:
gh codespace jupyter
```

### On your computer

Running tutorials on your computer requires some setup:

We recommend using [`pixi`](https://pixi.sh/latest/) to ensure a fully reproducible Python environment

```bash
git clone https://github.com/openalea/gallery.git
cd gallery
pixi run tutorial
```

If you prefer to use conda/mamba:

```bash
mamba env create -f .binder/environment.yml
mamba activate openalea-gallery
jupyter lab
```
