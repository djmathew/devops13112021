# Scenario 1 - Solution

## Objective

Print the numbers from 1 to 10 in random order to the terminal.

## Perquisites
1. Operating system required Linux or MacOS
2. Packages required:
   1. [git](https://github.com/git-guides/install-git) - to clone the repository from GitHub. Verify git is installed by the checking the installed version.
        ```shell
        git --version
        ```
        
   2. bash - to run the shell script. Verify if bash exists by look for the file /bin/bash
        ```shell
        ls /bin/bash
        ```
 
## Steps to run shell script    

1. Create a working directory
   ```shell
   mkdir djmathew
   ```
2. Move into the created directory
   
   ```shell
   cd djmathew
   ```
3. Clone the project repository from github 
   ```shell
   git clone https://github.com/djmathew/devops13112021.git djmathew-repo
   ```
4. Move to the cloned repo/directory
   ```shell
   cd djmathew-repo/scenario-1
   ```
3. Execute the bash script named `print-numbers.sh`

    ```shell
    ./print-numbers.sh
   ```
   or
   ```shell
    bash print-numbers.sh
   ```
> Expected outcome are the numbers 1-10 in a random order that doesn't repeat
