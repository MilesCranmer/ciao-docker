# [Bayesian X-ray Analysis (BXA)](https://johannesbuchner.github.io/BXA/) over [Chandra Interactive Analysis of Observations (CIAO)](http://cxc.harvard.edu/ciao/index.html) docker image:

## Acknowledgement

[Citing BXA](https://johannesbuchner.github.io/BXA/#citing-bxa-correctly)

[Citing CIAO](http://cxc.harvard.edu/ciao/) (bottom page)

## Default beaviour of the container:
Launched without option this container run the example script and open an image.

## How to run this image

On Linux:

`$ docker run -ti -v /tmp/.X11-unix:/tmp/.X11-unix -e DISPLAY=$DISPLAY ldouchy/bxa_ciao:latest`

/!\ you need to authorize the container to access your local X server. /!\

# Customise this image for your needs

In order to have CIAO working you need prior running your code to source the CIAO environement. 
The current install is made under root, LOGNAME variable is needed in order  to have a working CIAO. This will be fixed in the future by having a CIAO image without root installation:

`source /opt/ciao-4.7/bin/ciao.bash && export LOGNAME=root`

# BXA links

[BXA main page](https://johannesbuchner.github.io/BXA/)

