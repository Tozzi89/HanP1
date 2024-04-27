# About

This is a ESPHome firmware for the HanP1 devices created by [Tozzi89](https://github.com/Tozzi89/HanP1). the code is originaly from https://github.com/psvanstrom/esphome-p1reader, with some minor modifications (RGB LED support).

## Instructions
TBD

1. Use this repo template to [generate](https://github.com/esphome/esphome-project-template/generate) your own repository.
   - Make sure to check `Include all branches` so that GitHub Pages is automatically enabled.
2. Clone your new repository.
3. Add your project specific YAML configuration(s) along with the contents of the `project-template-....yaml` files, taking note of the comments in this template file and name accordingly.
4. 
    a. Update [.github/workflows/publish.yml](.github/workflows/publish.yml) to contain your own YAML config filename(s).
    b. Update [.github/workflows/ci.yml](.github/workflows/ci.yml) to contain your own YAML config filename(s).
5. Update [static/_config.yml](static/_config.yml) to change the title, description and basic theme of the generated website.
6. Add more content to the [static/index.md](static/index.md) file to explain your project.
    Make sure to leave the installation code tags in place so users get the install button.
7. Add permission to github-actions[bot]
   a. go to your project Settings, under the Actions collapsible, click on General.
   b. scroll down until you find Workflow permissions and mark the option Read and write permissions.
   c. Hit the save button
8. Push your changes to the repository and GitHub Actions will automatically build and deploy your project.
