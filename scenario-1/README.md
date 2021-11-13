# Scenario 1 - Solution

## Objective

Print the numbers from 1 to 10 in random order to the terminal.

## Perquisites
1. Operating system required Linux or MacOS
2. Packages required:
   1. [git](https://github.com/git-guides/install-git) - to clone the repository from GitHub

        ```shell
        # Verify git is installed
        git --version
        ```
        
   2. bash - to run the shell script
        ```shell
        # Verify if bash exists look for the file /bin/bash
        ls /bin/bash
        ```
 
## Steps to run shell script    

1. Create and move to a working directory
   ```shell
   # Create a directory name `djmathew`
   mkdir djmathew
   
   # Move into the created directory
   cd djmathew
   ```
3. Clone the project repository from github and move into the project directory
   ```shell
   # Clone the repository
   git clone https://github.com/djmathew/devops13112021.git djmathew-repo
   
   # Move to the cloned repo/directory
   cd djmathew-repo/scenario-1
   ```
3. Execute the bash script named `print-numbers.sh`

    ```shell
    ./print-numbers.sh
    # or
    bash print-numbers.sh
   ```
> Expected outcome are the numbers 1-10 in a random order that doesn't repeat