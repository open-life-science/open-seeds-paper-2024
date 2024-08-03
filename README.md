# Open Seeds paper 

This GitHub repository store sources (supplementary material, notebooks to generate figures) for the Open Seeds paper and its website.

## Running locally

### Requirements

- Install [conda](https://conda.io/miniconda.html)

    ```
    $ make install-conda
    ```

- Create the conda environment

    ```
    $ make create-env
    ```

### Generate figures

Jupyter Notebooks have been used to generate the graphs for the paper.

#### Usage

- Launch [Jupyter](https://jupyter.org/) to access the notebooks to generate graphs

    ```
    $ make run-jupyter
    ```

- Go to [http://localhost:8888](http://localhost:8888) (a page should open automatically in your browser)
- Open the interesting notebook

    For running the microgrants & honoraria notebook, you will need first to export the output of 2 searches on CiviCRM and add them in the `data/openseeds` folder to update files
    - `data/openseeds/honorarium.csv` by "Open Seeds honorarium" search
    - `data/openseeds/microgrants.csv` by "Open Seeds microgrants" search


- Make changes and save them

### Generate the website

- Run Jupyter book

    ```
    $ make build-jupyterbook
    ```

- Open `_build/html/index.html` in a browser

## License

Code is MIT, Content is CC-BY. 

 <p xmlns:cc="http://creativecommons.org/ns#" >This work is licensed under <a href="https://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY 4.0<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1" alt=""><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1" alt=""></a></p> 
