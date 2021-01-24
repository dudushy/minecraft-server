# minecraft-server
How to create and host a minecraft server from scratch.


[server.jar](https://www.minecraft.net/en-us/download/server/)

[Hamachi](https://www.vpn.net/)
[motd generator](https://minecraft.tools/en/motd.php)

create a text file named `start-server`

paste `java -Xmx0000M -Xms0000M -jar server.jar nogui` (change ram and version)

1gb /   -Xmx1024M -Xms1024M
2gb /   -Xmx2048M -Xms2048M
3gb /   -Xmx3072M -Xms3072M
4gb /   -Xmx4096M -Xms4096M
5gb /   -Xmx5120M -Xms5120M
6gb /   -Xmx6144M -Xms6144M
7gb /   -Xmx7168M -Xms7168M
8gb /   -Xmx8192M -Xms8192M
9gb /   -Xmx9216M -Xms9216M and so on... 1024 * Xgb

save the file as `.bat`

execute to setup

after setup
    agree to EULA