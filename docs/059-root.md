# Root
In the file systems, the directory structure is like a tree. We usually have the root node. In Unix, it is clearly the ‘/‘ folder is the root folder, from which everything starts. When it comes to windows, we C: or a drive name as the root folder.

Similarly, in projects, we have the PROJECT_ROOT folder. It’s the main folder in which the project code exists. This setting is used in the build processes, to specify the location at which it needs to start instead of the present working directory(PWD). When you type any command, the PWD will be taken as the directory to build from. Alternatively, you specify the root directory of the project from where you want to execute. This pattern is typical in many frameworks using which the apps are built. For this, some environmental variables are used like PROJECT_ROOT, PROJECT_OUTPUT. These specify the locations.

So, for example, when you start a nodeJS application, you need to run the commands from the project root directory.
