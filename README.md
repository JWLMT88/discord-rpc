# Python Discord Rich Presence Scripts
This repository contains a collection of Python scripts that allow you to display a Rich Presence on Discord. These scripts make use of the Discord RPC (Rich Presence Client) SDK, which is a powerful tool for integrating Discord into your applications.

## Requirements
To use these scripts, you'll need to have Python 3.6 or higher installed on your system. Additionally, you'll need to install the following Python packages:

- pypresence: This is the Python wrapper for the Discord RPC SDK. You can install it using pip:
```Python
pip install pypresence
```
## Usage
To use these scripts, simply clone this repository to your local machine:

```Python
git clone https://github.com/your_username/python-discord-rich-presence.git
```
Then, open the folder containing the script you want to use and run it using Python:
```Python
python script_name.py
```
## Available Scripts
- **__abelton.py__** : For more info open Ableton Directory

- **__game_time.py__** : This script displays the amount of time you've spent playing a particular game on Discord. To use this script, you'll need to specify the game's name and the time you started playing.

- **__spotify.py__** : This script displays the song you're currently listening to on Spotify as your Discord Rich Presence. You'll need to have the Spotify desktop app installed on your system for this script to work.

## Contributing
If you have an idea for a new script or would like to improve an existing one, feel free to submit a pull request! We're always looking for new ways to enhance the Discord experience.

### Tutorial

#### Import necessary libraries:

- pypresence: for updating Discord status
- random: for generating random numbers (unused in this script)
- ctypes: for accessing Windows API functions
- time: for getting the current time and waiting
- os: for running system commands and clearing the console

##### Set up variables:

- application_id: the ID of the Discord application used to update status
- title, program, and project: strings used to store window titles and project names
- btns: a list of buttons displayed on the Discord status
- Connect to Discord API using the Presence class from pypresence, and set the start time to the current time.

#### Enter a while loop that runs indefinitely:
- Use os.popen() to run the "tasklist" command and check if "Ableton Live 11 Suite" is in the output.
- If it is, clear the console and print a message indicating that Ableton is running.
- Define a function that uses the Windows API to get the title of the active window and extract the program and project names from it.
- Call the function and update the Discord status with the program and project names, the buttons, and the start time.
- If "Ableton Live 11 Suite" is not found in the output of the tasklist command, clear the console and print a message indicating that Ableton is not running.
- Wait for 10 seconds before checking again.

#### And that's it! This script continually checks if Ableton Live 11 Suite is running and updates the Discord status with the project name if it is.

## License
This repository is licensed under the MIT license. See the LICENSE file for more information.
