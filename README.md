# ⌨️ Macro Recorder

Simple console Python program made for recording and playing mouse and keyboard macros.

# Running

- Clone this repository.
- Install needed dependencies using:
```sh
pip install -r requirements.txt
```
- Run `main.py` using **Python**:
```sh
python main.py
```
- You may also want to pass the `--logging` argument to tell the program to show all of the information that's being gathered by the macro or played currently.
```sh
python main.py --logging
```

# Usage
- You can start recording by pressing `constants.RECORD_KEY` (in this case, F9).
- After you start the recording you can stop it by pressing `constants.STOP_KEY` (in this case, F10).
- Then, you can either play the recorded macro with `constants.PLAY_KEY` (in this case, F5) or record again with `constants.RECORD_KEY` (again, F9).
- You can save your macro by pressing `constants.SAVE_KEY` (in this case, F1) and writing a name for it (only if you have a macro already recorded currently).
- You can load any macro that is already saved by pressing `constants.LOAD_KEY` (in this case, F3) and writing its name. Macros are saved as JSON files in the `saves` folder.
- You can close the program by sending a **SIGINT** signal with `Ctrl + C`.