# Xenonstack_Technical_Task_1

Linux Custom Command:
I have provided screenshots on the above.
internsctl - Custom Command
internsctl is a custom command designed to perform various system operations and information retrieval tasks, simplifying administrative tasks and providing insights into system resources and users.

Functionalities:

User Operations:
createUser : Creates a new user if it doesn't exist. listRegularUsers: Lists regular users present on the system. listSudoUsers: Lists users with sudo privileges.
System Information:

cpu getinfo: Displays CPU information using lscpu. memory getinfo: Shows memory information using free.
File Information:

file getinfo [options] : Provides detailed information about a specified file. --size, -s: Print file size. --permissions, -p: Display file permissions. --owner, -o: Show file owner. --last-modified, -m: Print last modified details.
Usage:

To see the manual: internsctl man To display the version: internsctl --version For help on commands: internsctl --help
Setting up as a Custom Command:

To use internsctl as a custom command: Clone the repository or download the internsctl.sh file to your local system. Make the script executable: chmod +x internsctl.sh To run the command globally, move the file to a directory listed in your system's PATH. Example: /usr/local/bin/ You can use this command to move this file to system directory: sudo mv internsctl.sh /usr/local/bin/internsctl
Example Usage:
bash Copy code ./internsctl.sh user create JohnDoe ./internsctl.sh user list ./internsctl.sh user list --sudo-only ./internsctl.sh cpu getinfo ./internsctl.sh file getinfo --size hello.txt
