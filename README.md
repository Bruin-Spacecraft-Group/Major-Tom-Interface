## Purpose
This Python code gets data from the ground station (currently, a random number generator) and uploads it to the Major Tom dashboard. Barring the development of a custom website, this is the bridge connects the ground station (in the future, probably AWS) to "mission control."

## How to use
We stole example-python-gateway from the Kubos gateway repository: https://github.com/kubos/example-python-gateway. If you click on it, you will see a README that tells you how to link the code to a gateway in the "Gateway" list in https://app.majortom.cloud.

## Contributing
The code provided by Kubos does a lot of the heavy lifting of connecting & sending data already. What we have to do is:
- Change the data collection functions so that they pull data from the ground station instead of a random number function.
  - Most of these functions are in example-python-gateway/satellite/satellite.py. 
