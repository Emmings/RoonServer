# RoonServer
Dockerfile for RoonServer on Linux x86_64

Roon data files are stored in /var/roon. Music volume should be /music.

You currently must use the "host" networking driver with this.

Based on the version developed by mikedickey/roonserver

Example:

    docker run --name RoonServer --net=host -d -v /home/roon:/var/roon -v /home/music:/music Emmings/RoonServer
