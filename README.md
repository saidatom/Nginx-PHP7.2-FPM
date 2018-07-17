Nginx-PHP7.2-FPM
=============

This repo contains a recipe for making a [Docker](http://docker.io) container for Drupal, using Linux, Apache and PHP7.2-FPM. 
To build, make sure you have Docker [installed](http://www.docker.io/gettingstarted/).

This will try to go in line with [Drupal automated-testing](https://drupal.org/automated-testing).

## And run the container, connecting port 80:
```
sudo docker run -d -t saidatom/lep
```
That's it!
Visit http://localhost/ in your webrowser. 


## More docker

```
# sudo docker ps
ID                  IMAGE                   COMMAND               CREATED             STATUS              PORTS
9887DAS121        saidatom/lep:latest   /bin/bash /start.sh   3 minutes ago       Up 6 seconds        80->80  
```

Start/Stop
```
sudo docker stop 9887DAS121
sudo docker start 9887DAS121
```

## Authors

Created and maintained by [Alexandre Dias][author] (<alex.jm.dias_at_gmail.com>)

## License
GPL v3

[author]:                 https://github.com/saidatom

![](https://images.microbadger.com/badges/image/saidatom/lep.svg) ![](https://images.microbadger.com/badges/version/saidatom/lep.svg)
