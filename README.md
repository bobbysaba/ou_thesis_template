# University of Oklahoma Thesis/Dissertation Template

This template was created and is maintained by the **University of Oklahoma School of Meteorology Student Affairs Committee**. Created on 3 September 2025, this template implements Graduate College requirements as of that date. Documented changes to the template can be found in `VERSIONS.txt`. For the current thesis and dissertation formatting requirements, please refer to the [OU Graduate College Thesis/Dissertation Instruction Packet](https://www.ou.edu/content/dam/gradcollege/docs/gc-thesis-dissertation-instruction-packet.pdf).

## Downloading the Project from GitHub

To use this template, you can download the project files from GitHub to your local machine. Follow these steps:

1. **Download as a ZIP**:
   - Visit the repository on GitHub: [github.com/bobbysaba/ou_thesis_template](https://github.com/bobbysaba/ou_thesis_template.git).
   - Click the green **Code** button and select **Download ZIP**.
   - Extract the ZIP file to your desired local directory OR leave the .zip file as is to import into web applications such as Overleaf.
   - Navigate to the extracted `ou_thesis_template` folder to begin working with the template.

2. **Clone the Repository** (recommended for Git users):
   - Ensure you have Git installed (`git --version` to check).
   - Open a terminal and run:
     ```bash
     git clone https://github.com/bobbysaba/ou_thesis_template.git
     ```
   - This creates a `ou_thesis_template` folder in your current directory with all project files.
   - Navigate to the folder:
     ```bash
     cd ou_thesis_template
     ```

## Creating Your Thesis/Dissertation

Follow the steps below to set up and customize your document:

1. **Update Title Page Information**:
   - Open `0_title_pages.tex` and fill in the variables at the top of the file, including:
     - Document type
     - Degree
     - Program name
     - Paper title
     - Your name
     - Graduation year
     - Academic unit
   - In the second section of `0_title_pages.tex`, add your committee members.
     - feel free to comment/uncomment out pre-existing lines to match your number of committee members 
     - changes to this section must match the section beginning at line 82 of `0_title_pages.tex`
   - **Note**: Do not modify other parts of this file unless you intend to edit the template itself.

2. **Add Content to Document Files**:
   - Add your text to the following files:
     - `1_acknowledgments.tex`: Acknowledgments section
     - `2_abstract.tex`: Abstract section
     - `*.tex`: Your custom chapters
       - You may rename chapter files to reflect your chapter titles, but this is **not recommended** as it requires updating `main.tex` where these files are imported.
       - Comment out sections in chapters you will not use (see `7_other.tex` for an example).

3. **Tables, Equations, and Figures**:
   - Refer to `5_results.tex` for examples of how to insert tables, equations, and figures.

4. **Bibliography Formatting**:
   - This template uses the **American Meteorological Society** format for the bibliography (`ametsocV6.bst`).
   - **Do not edit** the `ametsocV6.bst` file, even if you choose a different citation format.
   - The OU Graduate College does not enforce a specific bibliography format, so you may use this or add your own (preferably in `.bst` format for compatibility with BibTeX/BibLaTeX).

## Forking and Contributing

If you’d like to make edits to the template and propose changes to the main branch, you can fork the repository and submit a pull request. Here’s how:

1. **Fork the Repository**:
   - On the GitHub repository page, click the **Fork** button (top-right corner) to create a copy of the repository under your GitHub account.
   - Clone your forked repository to your local machine:
     ```bash
     git clone https://github.com/bobbysaba/ou_thesis_template.git
     ```
   - Navigate to the cloned folder:
     ```bash
     cd ou_thesis_template
     ```

2. **Make Changes**:
   - Create a new branch for your changes:
     ```bash
     git checkout -b your-branch-name
     ```
   - Edit the necessary files (e.g., template files or documentation).
   - Stage and commit your changes:
     ```bash
     git add .
     git commit -m "Description of your changes"
     ```
   - Push your changes to your forked repository:
     ```bash
     git push origin your-branch-name
     ```

3. **Submit a Pull Request**:
   - Go to your forked repository on GitHub.
   - Click **Compare & pull request** next to your branch.
   - Provide a clear title and description of your changes.
   - Submit the pull request to the original repository’s `main` branch.
   - The maintainers will review your changes and may request revisions before merging.

4. **Syncing Your Fork** (optional):
   - To keep your fork updated with the original repository, add the upstream repository:
     ```bash
     git remote add upstream https://github.com/original-owner/github_repo.git
     ```
   - Fetch and merge upstream changes:
     ```bash
     git fetch upstream
     git checkout main
     git merge upstream/main
     git push origin main
     ```

## Notes
- Ensure you have LaTeX installed (e.g., TeX Live) or access to a web application (e.g., Overleaf) to compile the template.
- For questions about the template or contributions, contact the University of Oklahoma School of Meteorology Student Affairs Committee ([somsac@ou.edu](mailto:somsac@ou.edu)).