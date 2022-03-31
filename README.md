# gpages

## Script for the Workshop: Preamble

1. Set up a github account
2. Create a Public repository called `testgpages` with a `README.md` and a **Jekyll** `.gitignore`.
3. Clone this repository down.
4. Also fork-clone/clone the repository https://github.com/rahuldave/gpages . 
5. Open both repositories side by side in the Finder (File Manager)
6. Make an edit to the `README.md` in `testgpages` and commit and push to understand the git flow.

## Web Pages, Version 1

1. Copy the `notebooks` folder from `gpages` into `testgpages` (using the Finder or the terminal)
2. [OPTIONAL] Using that terminal, convert the notebooks to html: 
   1. `jupyter nbconvert --output-dir . --to html notebooks/olives-eda.ipynb`
   2. `jupyter nbconvert --output-dir . --to html notebooks/olives-model.ipynb`
3. Copy `oldondex.html` from `gpages` to `index.html` in `testgpages`. Edit to suit.
4. Commit and push
5. Go to the github user interface for settings and enable a website on the `master` branch of `testgpages`.
6. Go to `https://username.github.io/testgpages/index.html` to see your website


Notice that we have no navigation. We would have to build all this in by hand. Also notice the ugly `In` and `Out` prompts.

## Web Site Version 2

1. Delete the html files in the main `testgpages` folder. We will generate markdown instead
2. From `gpages` copy the `_layouts` folder, the _posts folder, the `_support` folder, `index.md`, and `_config.yml`.
3. Optionally add the `_support` folder to .gitignore so its not committed.
4. [OPTIONAL] Using the `testgpages` terminal, convert the notebooks into markdown using our custom template. Else use the provided markdown files.
   1. `jupyter nbconvert --output-dir . --to markdown --template _support/markdown.tpl notebooks/olives-eda.ipynb`
   2. `jupyter nbconvert --output-dir . --to markdown --template _support/markdown.tpl notebooks/olives-model.ipynb`
5. Commit and push and go to the website in a bit to see the changes we have got. Its much better already.
6. Add **YAML** preambles and some TOC frontmatter to our markdown files ( can do this by hand too)
   1. `python _support/nbmd.py olives-eda.md` 
   2. `python _support/nbmd.py olives-model.md`
7. Edit the markdown files to add a YAML tag `nav_include: 1` and `nav_include: 2` respectively to the above markdown files.The 1 and 2 reflect the position on the navigation menu in the `default.html` template in `_layouts`.  
8. Commit and push everything and go to the website in a bit to check the improvements

## Homework

Use the minimal-mistakes theme to create a portfolio site for yourself. You will have to create a repo: username.github.io

## More Info

- http://jmcglone.com/guides/github-pages/
