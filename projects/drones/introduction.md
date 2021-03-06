# Drones

## An introduction to the programming club's coolest assets

![Picture of a drone on the ground][drone on ground]

So you discovered the programming club has drones.

They can fly:
![Short clip of a drone flying][drone flying]
They can flip around:
![Short clip of a drone flipping over][drone flip]
And when you're lucky, they even land:
![Short clip of a drone landing][drone land]

There are many more features we may have a look at later, but getting a drone to take off, flip and land will be the focus of this introduction.

The best part of it all - you can get them to do this very easily yourself!
All you will need is:

- One of the DJI Tello drones
- A laptop with Python3 installed
  - If you don't have it yet, you can get it [here][Python page]

That's actually it. You don't even need to know Python to get started.

The first step to taming these drone beasts will be to turn one on.
If you pick drone, you will find that it has only one button - it is on the side opposite the charging port. Press this button for a second and it will turn on. While the drone is starting up, an LED indicator at the front will light up various colours and start flashing a steady yellow once ready.

Once the drone is ready to go, it will be broadcasting a WiFi network.
A sticker on the drone should say what the name of this network is.
Try connecting to the drone's network with your laptop.

Don't worry if your internet connection stops working - that's expected - the drone is not connected to the internet after all, this connection is just between your laptop and the drone.

Once you've gotten this far, you can connect back to the internet, we will reconnect to the drone later.

Visit the [Ryze Robotics page][Ryze page] on Tello drones to get the Tello SDK (software development kit) manual - click on the Tello SDK link on this website.

It should lead you to a PDF manual, on the first page of which, there will be a link to download a small Python template that will allow you to make the drone perform some basic tricks.

At the time of writing you could access the PDF [here][Tello SDK manual] and the Python template [here][Tello SDK template].

Once you have both, reconnect to the drone the same way you did before. Beware that it might have turned off in the meantime to save power (you will know by the LED indicator, which will still be flashing yellow if it is on).

When connected, run the Python script by opening up a terminal window, navigating to the folder where the script is and running `python <script name>`, where `<script name>` is the filename of the Python template file you downloaded.

It should display the following text (or similar if it changes in the future):

```shell
Tello Python3 Demo.

Tello: command takeoff land flip forward back left right 
       up down cw ccw speed speed?

end -- quit demo.
```

If you've played ahead of the game and taken a peek at the manual (and if not, then now) you will know that we will first need to set the drone to command mode before it can do anything.

Do this by typing `command` in the same terminal window.

This will attempt to tell the drone to switch to command mode and if successful, it will display `OK`.
If nothing comes up - here's a troubleshooting checklist:

1. Check that the drone is on (it might have turned off on its own)
2. Ensure you are connected to the drone's WiFi network
3. Make sure the python script did not show any errors when running it

If all else fails, ask one of the demonstrators, that's what they are here for! :)

Hopefully the drone will have a-OKed your command instruction, which means you can now make it takeoff!

This is as simple as typing `takeoff` in the terminal window.

You can then make the drone flip around using `flip f`, `flip b`, `flip r`, `flip l`, `flip fl`, `flip fr` commands.

You can make it land using, surprise surprise, the `land` command!

Finally, when you are done having fun, type `end` to exit the script.

If you ever get yourself in a situation, where you exited the script, but the drone is still in the air - just try running it again and typing `land` as if you were continuing.
If nothing seems to be working, don't panic - the drone will run out of battery rather quickly (usually they only last 10 minutes in the air on full battery) and land in self-preservation without you telling it to.

Read through the manual to see what else you can make the drone do ;)

![Picture of a drone in the air][drone in air]

That's all for the basic introduction. Check out the other worksheets (coming soon) for more advanced things you can do.

[drone on ground]: https://media.githubusercontent.com/media/Vidminas/pgclub-drone-media/master/jpg/drone%20on%20ground.jpg "One of those super cool drones!"
[drone flying]: https://media.githubusercontent.com/media/Vidminas/pgclub-drone-media/master/gif/takeoff.gif "Yes, they really do fly"
[drone flip]: https://media.githubusercontent.com/media/Vidminas/pgclub-drone-media/master/gif/flip.gif "Gets that wow reaction every time"
[drone land]: https://media.githubusercontent.com/media/Vidminas/pgclub-drone-media/master/gif/landing.gif "Fingers crossed you don't have to wait for the battery to run out"
[Python page]: https://www.python.org/downloads/
[Ryze page]: https://www.ryzerobotics.com/tello/downloads
[Tello SDK manual]: https://terra-1-g.djicdn.com/2d4dce68897a46b19fc717f3576b7c6a/Tello%20%E7%BC%96%E7%A8%8B%E7%9B%B8%E5%85%B3/For%20Tello/Tello%20SDK%20Documentation%20EN_1.3_1122.pdf
[Tello SDK template]: https://terra-1-g.djicdn.com/2d4dce68897a46b19fc717f3576b7c6a/Tello%20%E7%BC%96%E7%A8%8B%E7%9B%B8%E5%85%B3/Both/Tello3(1).py
[drone in air]: https://media.githubusercontent.com/media/Vidminas/pgclub-drone-media/master/jpg/drone%20in%20air.jpg "You've done it all! Congratulations"