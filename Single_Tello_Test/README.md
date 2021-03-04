# Single_Tello_Test
## Step 1

Place the commands which you would like to run in `command.txt`, for example:

```
command
takeoff
land
```

A full list of SDK commands is available on [the RYZE robotics website.](https://dl-cdn.ryzerobotics.com/downloads/Tello/Tello%20SDK%202.0%20User%20Guide.pdf)

## Step 2
The script will automatically send each command to the Tello. After receiving the reply from the previous command, the next command will be sent immediately.
To add a delay, you can use the `delay` command and the script will automatically delay for the specified amount of time. **The unit of delay is seconds**, and decimals are supported.

For example:

```
delay 5
```

## Step 3

Run the script:

```
python tello_test.py command.txt
```

  for Windows:
  
```
python.exe tello_test.py command.txt
```

The output window will display each instruction and its reply from the Tello. After execution of the script has finished, the commands sent and responses received will be written to a log file, named with the script end time.
