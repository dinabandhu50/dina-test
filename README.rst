*****************************
This is my first pypi package
*****************************

poetry 
------
- step 1: install poetry using 
    
    .. code-block:: sh
    
        curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python    

    before using the above code in Ubuntu system, you must set the default python to the version you want. Because by default python is set to version 2.7 in Ubuntu.

- step 2: Create a new project

    .. code-block:: sh 

        poetry new [project-name]
    
    The output will create a structured project. It will create a 'pyproect.toml' file also . This '.toml' file will have all the configuration for project.

- step 3: Some useful cli commands for poetry 
    
    .. code-block:: sh

        # add packages to project
            poetry add numpy, pandas 
        
        # checking
            poetry check 

        # build the package 
            poetry build 

        # publish to pypi 
            poetry publish 
        
        # venv of poetry 
            poetry shell

Poetry + Vscode
---------------

- step 1: open the project with vscode.

- step 2: Set the environment:

    .. code-block:: sh 

        // add the poetry venv directory path to vscode setting
            "python.venvPath": "~/.cache/pypoetry/virtualenvs"

        // now add the python path from down below bar of vscode 
        // to project env.

- step 3: Set the testing in vscode:

    .. code-block:: sh 

        // open command palette
            'ctrl' + 'shift' + 'p'

        // search for 'test' in command palette
            
        // choose the python test from drop down

        // Then select pytest from drop down 

        // In the down below of vscode a lightning 
        // 'Run test' will appear

        // In the left side of vscode a chemistry 
        // lab flask will appear for testing your tests. 
