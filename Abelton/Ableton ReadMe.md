# Ableton Live 11 Suite Discord Presence
This Python script uses the PyPresence library to update your Discord status based on whether Ableton Live 11 Suite is running. If Ableton Live 11 Suite is running, the script will update your Discord status with the name of the project you are currently working on.

## Setup
1. Install the PyPresence library by running the following command in your terminal:
```Python
pip install pypresence
```
2. Clone or download the **__ableton-discord-presence.py__** file from this repository to your local machine.

3. Open the **__ableton-discord-presence.py__** file in a text editor and replace the application_id variable with the ID of the Discord application that you want to use to update your status. You can find this ID on the Discord Developer Portal.

4. Save the ableton-discord-presence.py file.

## Usage
1. Open a terminal window and navigate to the directory where the ableton-discord-presence.py file is located.

2. Run the following command to start the script:
```Python
python ableton-discord-presence.py
```
3. If Ableton Live 11 Suite is running, the script will update your Discord status with the name of the project you are currently working on. If Ableton Live 11 Suite is not running, the script will wait for 10 seconds before checking again.

4. To stop the script, press Ctrl + C in the terminal window.

## Customize
If you want to customize the buttons that are displayed on your Discord status, you can modify the **__btns__** variable in the **__ableton-discord-presence.py__** file. You can add or remove buttons as needed.

```Python
Copy code
btns = [
    {
        "label": "Live 11 Suite",
        "url": "https://www.ableton.com/en/shop/live/"
    },
    # Add more buttons here
]
```
## License
This script is licensed under the MIT License.
