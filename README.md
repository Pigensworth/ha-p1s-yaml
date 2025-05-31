## Here's my setup for my Bambulab P1S in Home Assistant. I'm still working on getting the AMS working, so beware.

![image](https://github.com/user-attachments/assets/12ab9d4a-4761-486f-99ae-45cbff28e4d2)

# Setup
## Main Screen
For the main screen, create a new dashboard, go to **edit dashboard -> edit view -> edit in yaml** and replace everything in there with the contents of [p1s_main_screen.yaml](https://github.com/Pigensworth/ha-p1s-yaml/blob/main/p1s_main_screen.yaml). It will throw some errors to start with, but that will be fixed later.

## Automations
Create a new automation, edit in yaml, and replace it with [print.yaml](https://github.com/Pigensworth/ha-p1s-yaml/blob/main/print.yaml). Repeat with [update_filename.yaml](https://github.com/Pigensworth/ha-p1s-yaml/blob/main/update_filename.yaml)

## Helpers
To create a helper, go to **Ssetting -> Devices & services -> Helpers -> Create Helper**. Below is a list of names for each type of helper.

### Input Datetime
start_date_time

### Input Boolean
ams_toggle, bed_leveling, start_print, timelapse, start_now.

### Input Select
part, ams_1, ams_2, ams_3, ams_4

### Input Text
file_name
