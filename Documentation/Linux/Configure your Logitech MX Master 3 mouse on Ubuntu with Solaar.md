[  
Freedium](https://freedium.cfd/)

- [ko-fi](https://ko-fi.com/zhymabekroman)
- [librepay](https://liberapay.com/ZhymabekRoman/)
- [patreon](https://patreon.com/Freedium)

[< Go to the original](https://medium.com/@tihomir.manushev/configure-your-logitech-mx-master-3-mouse-on-ubuntu-with-solaar-407f76f4890e#bypass)

![Preview image](https://miro.medium.com/v2/resize:fit:700/1*RGTcL-otZjmkDeiUN8jnlA.jpeg)

# Configure your Logitech MX Master 3 mouse on Ubuntu with Solaar

## Intro

[![Tihomir Manushev](https://miro.medium.com/v2/resize:fill:88:88/1*ue4qCDynN3l-hO6NJoKlLw.jpeg)

](https://medium.com/@tihomir.manushev "Backend Developer at Generic Soft")

[Tihomir Manushev](https://medium.com/@tihomir.manushev "Backend Developer at Generic Soft")[Follow](https://medium.com/@tihomir.manushev "Backend Developer at Generic Soft")

androidstudio·May 24, 2024 (Updated: May 24, 2024)·Free: No

### Intro

At the time of writing this article, Logitech is still refusing to provide it's Logi [Options](https://www.logitech.com/en-eu/software/logi-options-plus.html)+ software for Linux. This means that if we want to customize our MX Master mouse (or other Logitech products) we'll need to use third party tool. One of the best such tools is Solaar, but is requires some manual configuration that some users may find too confusing. Fear not, I'm here to help!

### The docs

[This](https://github.com/pwr-Solaar/Solaar) is the official GitHub repo of Solaar. Have a look if you encounter some issues.

[This](https://pwr-solaar.github.io/Solaar/index) is the Solaar documentation. It offers more in-depth information about the tool.

### Installation

Let's begin with the installation. I will use Ubuntu 24.04 and a MX Master 3S mouse.

Copy/paste the following commands in the terminal:

Add the PPA. A Personal Package Archive (PPA) is a software repository specifically made for Ubuntu users. PPAs are used by developers to distribute their software.

Copy`sudo add-apt-repository ppa:solaar-unifying/stable sudo apt-get update`

Now install Solaar

Copy`sudo apt install solaar`

Great, we now have Solaar installed! But we are not done yet. Go to the apps list and click the Solaar icon

![None](https://miro.medium.com/v2/resize:fit:700/1*c6pN6BVkAuzbiO8fVLqJqg.png)

Search for solaar in your apps list

The app will launch and.. the MX Master mouse is not detected.

![None](https://miro.medium.com/v2/resize:fit:700/1*KqWa4peIZAcyIeLGPk_JVg.png)

Don't worry, just unplug the mouse receiver and plug it again to the computer.

![None](https://miro.medium.com/v2/resize:fit:700/1*qTu0acOeB3Fg5ZlQo0BdUQ.png)

The Solaar GUI

Here Solaar successfully detected my G502, ERGO K860 and MX Master 3S.

### Customizing the mouse buttons

I will now show you how to customize the thumb scroll for volume up/down, the back and forward buttons (those are right under the thumb scroll wheel) for copy/paste. Of course you can customize those or other buttons to whatever you want.

Have a look at the previous screenshot of the Solaar GUI and adjust the toggle buttons accordingly. You can click on the lock icon next to each toggle button/setting to unlock it and edit it.

The most important setting for the volume up/down customization is `Thumb Wheel Diversion` . This is what will allow us to customize the thumb wheel behavior.

Another important setting is `Key/Button Diversion` . This will allow us to change the default behavior of the back and forward buttons. Unlock it and pick `Back Button` from the left dropdown menu, then pick `Diverted` from the right dropdown menu.

![None](https://miro.medium.com/v2/resize:fit:700/1*YHCFnkCSJU78dX3cWlayOA.png)

Divert the back button

Now do the same with the `Forward Button`

![None](https://miro.medium.com/v2/resize:fit:700/1*EyN_cVLFEtMj4gg1I9Rb8A.png)

Divert the forward button

Now lock the `Key/Button Diversion` option.

Next we need to add some custom rules for the thumb wheel and the two buttons. To do so click the `Rule Editor` button in the bottom right corner of the Solaar app. A new window will open containing the user defined riles (currently empty) and the built in rules.

Right click on the `User-defined rules` and choose `Insert new rule`

![None](https://miro.medium.com/v2/resize:fit:700/1*i4F-WGwDL9-VUDE_PD7Jvg.png)

Now right click on `[empty]` and choose `Insert here` -> `Sub-rule`

![None](https://miro.medium.com/v2/resize:fit:700/1*Li9VvetxaOACt1M2xEwQew.png)

Right click on `[empty]` and choose `Insert here` -> `Condition` -> `Test`

![None](https://miro.medium.com/v2/resize:fit:700/1*iawV6grJEfVLjn5g0k9GfA.png)

Type `thumb_wheel-up` in the left input field (Test) and choose a value for the scroll speed in the right input field (Parameter)

![None](https://miro.medium.com/v2/resize:fit:700/1*pldCfet_fVAhA3-JEZZ7Rw.png)

Now right click on `Test` and choose `Insert below` -> `Action` -> `Key press`

![None](https://miro.medium.com/v2/resize:fit:700/1*ew-NI1zshgvuor2kkoBWqA.png)

Now type `audioraisevolume` in the input field and choose `XF86_AudioRaiseVolume` .

![None](https://miro.medium.com/v2/resize:fit:700/1*C36kGnKHTZjucQbb1za1FQ.png)

At this point it will be a good idea to turn off your speakers because right now if you scroll the thumb wheel, the volume will hit 100% almost instantly. This is because we need to set some permissions in the next step.

Next we need to add a sub-rule for the `thumb_wheel_down` and `XF86_AudioLowerVolume` . The process is identical so I will screenshot the first steps without further explanations.

![None](https://miro.medium.com/v2/resize:fit:700/1*JyLs7tm6EkQAG6XsQ4tlgg.png)

![None](https://miro.medium.com/v2/resize:fit:700/1*np93cNhSgyD-yOf5USFyiw.png)

This is how it should look with the two sub-rules set up

![None](https://miro.medium.com/v2/resize:fit:700/1*tpvytzQweO5F5dbWgOR0AQ.png)

Now we can create two separate rules for the copy/paste functionality.

![None](https://miro.medium.com/v2/resize:fit:700/1*dNFZyMIltLY2VkvWMmP3Ig.png)

![None](https://miro.medium.com/v2/resize:fit:700/1*z2usPiI7W-VG0LZM2aRH6g.png)

![None](https://miro.medium.com/v2/resize:fit:700/1*VuQ_Fjf2iIoY_x-iRaC5zw.png)

![None](https://miro.medium.com/v2/resize:fit:700/1*3tr455u_4cx_uIIe-jDidw.png)

Type `Control_L` in the left input field and `c` in the right input field. This will map the forward button to `CTRL + c` or copy.

![None](https://miro.medium.com/v2/resize:fit:700/1*wSveXb06SAU-7jdQ0R47Tg.png)

Now repeat the process for the back button (paste)

![None](https://miro.medium.com/v2/resize:fit:700/1*oOtDUYFbLBGth5hYyXZppw.png)

The final setup should look like this

![None](https://miro.medium.com/v2/resize:fit:700/1*DS4A-lNN-fGfxr1Mwxx0lw.png)

You can now click the `Save changes` button in the top of the window and close it.

### The permissions

Solaar needs write access to `/dev/uinput` . The documentation states

> The easiest way to maintain write access to /dev/uinput is to use Solaar's alternative udev rule by downloading [https://raw.githubusercontent.com/pwr-Solaar/Solaar/master/rules.d-uinput/42-logitech-unify-permissions.rules](https://raw.githubusercontent.com/pwr-Solaar/Solaar/master/rules.d-uinput/42-logitech-unify-permissions.rules) and copying it as root into the /etc/udev/rules.d directory.

To do so we can execute the following commands in the terminal

Download the udev rule file:

Copy`wget https://raw.githubusercontent.com/pwr-Solaar/Solaar/master/rules.d-uinput/42-logitech-unify-permissions.rules`

Copy the file to the udev rules directory: You need root permissions to copy the file into the `/etc/udev/rules.d` directory. Use `sudo` to perform this operation.

Copy`sudo cp 42-logitech-unify-permissions.rules /etc/udev/rules.d/`

Reload udev rules: After copying the rule file, reload the udev rules to apply the changes.

Copy`sudo udevadm control --reload-rules`

Trigger the udev rule: Optionally, you can trigger the udev rule for the device without rebooting.

Copy`sudo udevadm trigger`

This should do the trick and you should now have customized your MX Master 3 mouse.

### GNOME extension

Additionally, on Wayland you can install the Solaar Extension for GNOME from [here](https://extensions.gnome.org/extension/6162/solaar-extension/).

### Conclusion

Solaar gives us way more options for customizing our Logitech devices. Feel free to explore the documentation and to experiment with the rules.

If you find this article helpful, please give it a clap. If you have a question, don't hesitate to leave a comment.

Thank you.

[#linux](https://medium.com/tag/linux "Linux")[#logitech](https://medium.com/tag/logitech "Logitech")[#mx-master](https://medium.com/tag/mx-master "Mx Master")[#ubuntu](https://medium.com/tag/ubuntu "Ubuntu")[#tutorial](https://medium.com/tag/tutorial "Tutorial")