# AUTO ACCEPT COUNTER STRIKE GLOBAL OFFENSIVE SCRIPT BY Shakshooka_
from pyautogui import *
import time
import pyautogui
import keyboard
import random
import win32api, win32con
pyautogui.FAILSAFE=False

# X:  960 Y:  416 RGB: ( 90, 203,  94)
# X:  957 Y:  502 RGB: ( 76, 175,  80)

def click(x,y):
    win32api.SetCursorPos((x,y))
    win32api.mouse_event(win32con.MOUSEEVENTF_LEFTDOWN,0,0)
    time.sleep(0.1)
    win32api.mouse_event(win32con.MOUSEEVENTF_LEFTUP,0,0)

while 1:
    if keyboard.is_pressed('q'):
        break
    if pyautogui.pixel(960, 416)[0] == 90 and pyautogui.pixel(960, 416)[1] == 203 and pyautogui.pixel(960, 416)[2] == 94:
        click(960, 416)
        print("Match is accept enjoy ez win :D")
        time.sleep(0.5)
    else:
        print("I am no see accept")
        time.sleep(0.5)
    if pyautogui.pixel(960, 416)[0] == 76 and pyautogui.pixel(960, 416)[1] == 175 and pyautogui.pixel(960, 416)[2] == 80:
        click(960, 416)
        print("Match is accept enjoy ez win :D")
        time.sleep(0.5)
    else:
        print("I am no see accept")
        time.sleep(0.5)
