# minecraft-server
How to create and host a minecraft server from scratch.

<details open>
<summary>Topics</summary>

- [Dependences](#depedences)

- [Create network](#create-network)

- [Create server](#create-server)

- [Open server](#open-server)

- [FAQ](#faq)
</details>

---
<details open>
<summary><a name="dependences" style="pointer-events: none;"></a>Dependences</summary>

- [server.jar](https://www.minecraft.net/en-us/download/server/)

- [Radmin VPN](https://www.radmin-vpn.com/)

</details>

---
<details open>
<summary><a name="create-network" style="pointer-events: none;"></a>Create network</summary>

1. Open `Radmin VPN`.

2. Create a network.
    
    _You may need to sign in/sign up._
    - Click on `Network`.

        ![network](https://i.imgur.com/u3m3ev5.png)

    - Click on `Create New Network`
    
        ![create_network](https://i.imgur.com/o315gv6.png)

    - Give your network a name and a password.

        ![network_name_and_password](https://i.imgur.com/GMRPjAV.png)

3. Copy IPv4. :warning:
    - Right click on your name and copy IPv4 address.

        _Save your IPv4, you will use on the server!_

        ![copy_ipv4](https://i.imgur.com/C9pI7FZ.png)

4. We're done here! :smile:

</details>

---
<details open>
<summary><a name="create-server" style="pointer-events: none;"></a>Create server</summary>

1. Create a folder for your server.

2. Download [server.jar](https://www.minecraft.net/en-us/download/server/) to your server folder.

3. Inside the folder, create a text file named `start-server`.
    - Before pasting the command line below, choose how much RAM you want to use:

        `-Xmx` is how much memory it's allowed to use.

        `-Xms` is the initial memory size (no performance impact).

        ```
        1gb /   -Xmx1024M -Xms1024M
        2gb /   -Xmx2048M -Xms2048M
        3gb /   -Xmx3072M -Xms3072M
        4gb /   -Xmx4096M -Xms4096M
        5gb /   -Xmx5120M -Xms5120M
        6gb /   -Xmx6144M -Xms6144M
        7gb /   -Xmx7168M -Xms7168M
        8gb /   -Xmx8192M -Xms8192M
        9gb /   -Xmx9216M -Xms9216M and so on... just multiply 1024 for how much you want
        ```

    - Paste `java -Xmx2048M -Xms1024M -jar server.jar nogui` (change RAM for your preference)

    - Save the file as `.bat`

4. Execute `start-server.bat` to setup.
    - When the console says `[Server thread/INFO]: Done! For help, type "help"` type `stop` to close.

        _The program may close itself automatically._

5. After setup, open `eula.txt` and agree to EULA:
    - `eula=true`

6. Execute `start-server.bat` to actually install the server.
    - When the console says `[Server thread/INFO]: Done! For help, type "help"` type `stop` to close.

        _Now you should have a lot of files and folders._

7. Edit `server.properties`.
    - Usually, we change those:

        `gamemode=` survival/creative/adventure/spectator

        `difficulty=` peaceful/easy/normal/hard

        `pvp=` true/false

        `hardcore=` true/false

        `enable-command-block=` true/false

        `max-players=` default=20

        `server-ip=` YOUR_HAMACHI_IPV4 :warning:

        `level-name=` default=world

        `online-mode=` true/false (`false` allows cracked)

        `level-seed=` leave empty for random seed

        `motd=` default=A Minecraft Server / ([motd generator](https://minecraft.tools/en/motd.php))

8. Well, we're done! :smile: ~~I love adding a new step just to tell you we're done~~

</details>

---
<details open>
<summary><a name="open-server" style="pointer-events: none;"></a>Open server</summary>

1. Just execute `start-server.bat`.

2. Guess what? We are done! :smile:

</details>

---
<details open>
<summary><a name="faq" style="pointer-events: none;"></a>FAQ</summary>

- How to change server ip?

    _Open `server.properties` and change `server-ip=` to whatever you want._

- How to add/change server world?

    _Open `server.properties` and change `level-name=` to whatever you want, it will create a folder with the name of level. Yes, you can have multiple levels in the same server folder, to rotate the maps you just need to change `leve-name=` to the folder name._

- What are the commands to use in console?

    _Well, there are a LOT of commands you can use, I recommend [this site](https://minecraft.gamepedia.com/Commands)._

</details>

---
> [GO BACK TO TOP](#minecraft-server)