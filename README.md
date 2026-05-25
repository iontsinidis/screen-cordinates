# screen-cordinates
a code where you can see where your cursor is pointing
import pyautogui
import time

print("Πατα CTRL+C για εξοδο.\n")

try:
    while True:
        x, y = pyautogui.position()
        print(f"\rΚερσορας: X={x} Y={y}", end="")
        time.sleep(0.05)

except KeyboardInterrupt:
    print("\nΤο προγραμμα σταματησε.")
