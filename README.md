# Problem with OpenGL and Wayland
 # If you don't want to type all the text here is the solution
 Problem: Wayland (Specifically XWayland)
 Solution: Change session to an X11 session
 # History
 ## Context

 When using Makehuman under Wayland, I encountered a problem with OpenGL, where the application did not run properly. After several tests and research, I discovered that the problem came from the Wayland server itself, which did not manage the OpenGL contexts well for certain applications like Makehuman.

 ## Solution

 ### 1. Go to X11

 The simple solution was to go to X11 instead of Wayland. To do this:
 1. Disconnect your Wayland session.
 2. Choose ** Plasma (X11) ** or another X11 session to connection.
 3. Relaunch Makehuman, and everything worked correctly.

 ### 2. Install XWayland (if you want to stay on Wayland)

 If you want to continue using Wayland, you can install XWayland, which allows you to run X11 applications under Wayland:
 `` bash
 Sudo Pacman -s Xorg -Xwayland
(or any other commmands, depends on your distro)
# Author's end message (it's me;) )
 For information I used this "Software Setup" to the time of this error

 OS: Arch Linux X86_64 [6.11.7-Arch1-1]
 Makehuman version: 1.3.0 Alpha

## I hope it will serve
