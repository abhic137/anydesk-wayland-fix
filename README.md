# anydesk-wayland-fix
Way 1. Disable Wayland in GDM3

To begin, you can disable Wayland in the GDM3 (GNOME Display Manager) custom configuration file.

Step 1. Open the terminal by pressing Ctrl + Alt + T.

Step 2. Type the following command to open the GDM3 configuration file in a text editor with administrative privileges:

sudo nano /etc/gdm3/custom.conf

gdm3

Step 3. Locate the [daemon] section in the file and uncomment the line "WaylandEnable=false".

Step 4. Modify the line "AutomaticLogin=user1" to "AutomaticLogin=$USERNAME" (replace "$USERNAME" with your actual username).

Step 5. Uncomment the two lines "AutomaticLoginEnable=true" and "AutomaticLogin=$USERNAME". Save the changes.

daemon

Step 6. Finally, reboot your Ubuntu server to apply the changes and allow them to take effect.
