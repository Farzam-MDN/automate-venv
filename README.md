# automate-venv



<!---
![automate-venv Logo](https://i.imgur.com/kDqIlrb.png)
-->


This repository contains files that help automate your virtual environments in python. Using the information and the files provided you can automatically create virtual environments, run virtual environments, run your scripts in virtual environments and do pip freeze command (which creates the requirements.txt file).


## Getting Started

These instructions will get you a copy of the project up and running on your local machine.

### Prerequisites

You need the following in order to automate virtual environments on your machine:

```
Python 3 or above (The commands have not been tested yet with python 2 and below)
```

### Automating virtual environments

First clone this repository or download it manually to a working directory on your computer.
Now make a new directory on your computer for an example project you want to automate (I name the directory 'exampleproject').
copy and paste the contents of 'automate-venv' directory into the 'exampleproject' directory.
Now run 'venvcreator.bat' file inside the 'exampleproject' directory.
Wait until the command prompt shows a timeout message and closes itself. 
Now a virtual environment called 'venv' has been created in 'exampleproject' directory.
Make an example python file in 'exampleproject' directory (I name the file 'example.py'). This is the file you will later on run inside the virtual environment automatically.
Edit the 'runscript.bat' file located in 'exampleproject' directory. In the first line of the 'runscript.bat' file you see a location path followed by cd command. Replace the location path with the full path to you scripts folder in 'exampleproject' directory (navigate to exampleproject/venv/scripts and copy the full location path). The location path that you enter in the 'runscript.bat' file should use backslashes '\'. 
Now copy the first line of the 'runscript.bat'. Edit 'runvenv.bat' and replace the first line of it with the copied line from 'runscript.bat'. Edit 'autopipfreeze.bat' and replace the first line of it with the copied line from 'runscript.bat'
Edit the 'addtoactivateautobat.txt' file. As you can see on the third line name of the example python file is mentioned ('example.py'). We don't change the name of the python file in this demo. But in case you are automating your own python file you need to replace 'example.py' with the full name of your python script.
Navigate to exampleproject/venv/scripts. copy and paste the 'activate.bat' file in the scripts folder. Now rename the pasted file to 'activate-auto.bat'. Make another copy of 'activate.bat' in scripts folder and paste it in the same directory. Now rename the pasted file to 'pipfreeze.bat'. 
 
 Now navigate to 'exampleproject' directory. Copy all the text inside 'addtoactivateauto.txt' into your clipboard. navigate to exampleproject/venv/scripts and edit the 'activate-auto.bat' file. Now paste what you copied before at the end of the 'activate-auto.bat' file.
 
 Lastly navigate to 'exampleproject' directory. Copy all the text inside 'addtopipfreeze.txt' into your clipboard. navigate to exampleproject/venv/scripts and edit the 'pipfreeze.bat' file. Now paste what you copied before at the end of the 'pipfreeze.bat' file.

**Your virtual environment is now automated!**

>Navigate to 'Exampleproject' directory.
To run the environment, open 'runvenv.bat'.
To run the 'example.py' file inside the environment, open 'runscript.bat'.
To make a 'requirements.txt' file for your environment, open 'autopipfreeze.bat'.


## Contributing

Feel free to fork and expand this project! Send a pull request if you would like to add your code to the project.

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/farzammadani/JustShareKeys/releases). 

## Authors

* **Farzam Madani** - *Creation of the core application* - [farzammadani](https://github.com/farzammadani)

See also the list of [contributors](https://github.com/farzammadani/JustShareKeys/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.md](https://github.com/farzammadani/JustShareKeys/blob/master/LICENSE) file for details

## Acknowledgments

* Big thanks to anyone who likes things automated!
