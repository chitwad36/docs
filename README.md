# Branch Docs

## Production

- https://branchmetrics.github.io/docs/

## Contributing 

- #### Best practices
    - Educate with `working code examples`.
    - `Bullet point` key points, procedures, and steps.
    - Use `shorter sentences with simpler words` (3rd grade reading level).
    - Write in the viewpoint of the `user`, not Branch.
    - Keep is simple (KISS) (`1 -> 2 -> 3`)
    - Don't repeat yourself (DRY) (`this can be found here`)

- #### Folders
    - Must be lowercase and hyphened

- #### Content
    - Bullets and sections must have new line spacing in between
    - Indention is 4 spaces
    - Search works best when content is not duplicated
    - Only add periods if more than one sentence

- #### Style
    - titles `# Title`
    - sections `## Section` 
    - category `- #### Section` 
    - content `    - content` 

- #### Search
    - Hosted by [Algolia Docsearch](https://community.algolia.com/docsearch/)
    - Localhost scrapes production
    - Production is scraped once a day

- #### Images
    - Content pages are kept in the `img/pages` 
    - Example images used in ingredients are kept in the `img/ingredients` 

- #### Includes 
    - For reusable snippet, use the format `{! path/file_name_here.md !}` 
    - Content snippets should be placed in the `ingredients` subdirectory
    - Frequently updated content/code should be kept within the `includes`

## Development

- #### Dependencies

    ```bash
    python --version #Python 2.7.2
    pip --version #pip 1.5.2
    ```

- #### Code

    ```bash
    git clone git@github.com:branchmetrics/docs.git
    cd docs
    ```

- #### Extensions

    ```bash
    pip install --upgrade pip
    pip install --editable lib/mkdocs
    pip install pygments
    pip install pymdown-extensions
    pip install markdown-include
    pip install mkdocs-material
    ```

- #### Develop

    ```bash
    mkdocs serve
    ```

    - http://localhost:8000

- #### Deploy

    ```bash
    mkdocs gh-deploy
    ```

    - https://branchmetrics.github.io/docs


## Resources

- http://www.mkdocs.org/

- https://github.com/squidfunk/mkdocs-material

- https://github.com/facelessuser/pymdown-extensions


## Additional

- modify mkdocs
    - readme http://www.mkdocs.org/about/contributing/
    - update to repo `git subtree add --prefix lib/mkdocs https://github.com/mkdocs/mkdocs master --squash`
    - add locally `pip install --editable lib/mkdocs`
    - remove locally `sudo rm /usr/local/bin/mkdocs && rm /Library/Python/2.7/site-packages/mkdocs.egg-link`

- modify mkdocs-material
    - readme http://squidfunk.github.io/mkdocs-material/customization/#theme-development
    - update to repo `git subtree add --prefix lib/mkdocs-material https://github.com/squidfunk/mkdocs-material master --squash`
