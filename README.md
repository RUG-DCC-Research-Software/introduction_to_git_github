# Introduction to Git & GitHub Workshop

This repository contains the followings:
- The presentation given on 21/10/2025 during the DCC Workshop: Introduction to Git & GitHub Workshop part 1
- A README file where the first part of homework is explained
- A data file to use for exercise purpose.


### Reminders
1) Make sure that you have a GitHub account and created a ssh key
2) **Optional**: On VS code, make sure that;

    `Source Control` pane works 

    `git graph` extension is installed on VS Code

If you are using another IDE such as PyChram or a differnt GUI, then install an extension equivalent to `git graph`.

### Steps
1) On the GitHub repository click on the green drop down menu on the right called <> Code.
2) Copy the HTTPS addres of the repository to clone
3) On your terminal in VS Code, to a directory of your choice, clone this repository by running the following command:

`git clone https://github.com/RUG-DCC-Research-Software/introduction_to_git_github.git`

4) Check the content of the repository. You should see the following files and folders:

`20102025-Introduction_to_git_github.ppx`: The presentation of the forst half of training.

`README.md` : READMe file that explains the steps of the first home work.

`data/data.csv`: A data file where the columns contains, tiemstamp, categorical labels and continues values.  


## Home Work 1

For the first part you will work on the local copy of the repository in your laptop.

The goal of the home work is for you to get familair with daily git workflow that consists of frequent commits and , working with branches and monitoring the commit history. You will use the `data.csv` file, making basic statistical analysis and visualize them. 

You can use any programming language of your choice. The goal is not to assess your programming skills, but to simulate a simple work case that you might have in your project.

You can use the presentation or the other sources to get help.

**Optional**: In VS Code, or on the IDE you work with, activate the `Source Control` pane and launch the `git graph` extension. It will visualize how your branches and commit history progress. Do not use the short cuts given in the `Source Control`, instead always type your commands in the terminal.

1) Check the content of the `.gitignore` file. If you want to add files or folders in your local repository that you don't want git to track, than add the names to the `.gitignore` file.
2) Make sure to not track or add sensitive information.

### Analyse data 1

1) Create and switch to the branch `analyse`.
2) Create a folder name `analysis`. 
3) In the `analysis` folder start developing a script that calculates mean and std for `value` and `category` and save to csv file under `outputs/summary.csv` 
4) Stage & commit the small changes frequently, not less than 4. Always check the status of the branch you work in.
5) Compare the status of the file or the repository before and after staging, or compare it with the `master` branch.
6) Compare different commits.
7) Can you interpret the how `git` displays the differences and makes comparison?
8) Delete the `summary.csv` and then restore it.
9) If your script successfully creates the desired output and your branch is in order then merge `analyse` branch to `master`.

### Plot data 1

1) If the merge is successfull, then create and switch to another branch called `plot`.
2) Create a folder name `plots`. 
3) In the `plots` folder start developing a script that creates ditsribution plots such as histograms/KDEs overall and per category, and save the plots under the folder `plots`.
4) Stage & commit the small changes frequently, not less than 4. In between compare your working branch with `master` and `analyse`.
5) If your script successfully creates the desired output then merge you branch to `master`.

### Analyse data 2

1) If the merge is successfull, then switch back to `analyse`.
2) In the `analysis` folder, create separate script that looks for a relation between `value` and `time`.
3) Save the plot(s) that diplay the relation and fitting in the folder `plots`. 
4) Stage & commit the small changes frequently. 
5) Compare differnet branches and compare the status of the file(s) between different commits and stages.
6) if your script(s) works as desired, the merge your branch to `master`.









