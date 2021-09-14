# GestureVolumecontrol
Gesture Volume control using OpenCV and using mediapipe framework
install openCV using pip command --> pip install openCV
install mediapipe using pip command ---> pip install mediapipe
or
If you are using pycharm you can just simply install it from the settings menu
Later you need to install pycaw by using --> pip install pycaw
or same as mentioned on line 6
pycaw(Developed by AndreMiras is the best module you can find and is the most used)
pycaw usage code is given below

from ctypes import cast, POINTER
from comtypes import CLSCTX_ALL
from pycaw.pycaw import AudioUtilities, IAudioEndpointVolume
devices = AudioUtilities.GetSpeakers()
interface = devices.Activate(
    IAudioEndpointVolume._iid_, CLSCTX_ALL, None)
volume = cast(interface, POINTER(IAudioEndpointVolume))
volume.GetMute()
volume.GetMasterVolumeLevel()
volume.GetVolumeRange()
volume.SetMasterVolumeLevel(-20.0, None)



THANK YOU
