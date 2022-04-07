# MagneticTimeCrystals

## Requirements

```sh
pip3 install -r requirements.txt
```
`ffmpeg` must be installed **and** in your path if you wish to run `video.py`. 
It is recommended to have `gcc` installed and in your path, so that you can use the C implementations of certain functions which speed up the program significantly (400%). Simply run the makefile and then continue to run the model as normal.
## Running Models
Choose a model/simulation from the `models/` folder.
* `temp_v_magnetisation.py` -- a plot of final magnetisations at a range of temperatures
* `video.py` -- a video visualisation of the evolution of the system
* `tau_v_mu_temp.py` -- plots a matrix of final magnetisation for a range of tau and mu values, can be useful for determining the boundary of time crystal behaviour
NOTE: Windows users may have to move the files inside of the `models/` folder out into the main folder, as windows does not handle symbolic links very well

# TODO
Once something has been completed, add it to `CHANGELOG.md` with the date and some brief description, and tick it off on the TODO list. Feel free to add anything.

- [ ] Add arguments to be taking in when running file
- [x] Custom starting shapes of a particular spin e.g. stars/circles through the use of image rasterisation
- [x] Add proper axes to `tau_v_mu.py`
- [x] Make a plot as seen in the Gambetta paper 2.(d)
- [x] Add ability to simultaneously flip a certain amount of spins  
- [x] Implement oscillations in time (because it is a time crystal)
- [x] Add a magnetic field that favours either spin up or down
- [x] Add ability to export just graphs where parameters change e.g. Magnetisation vs Temperature - would need to find the number of cycles until it roughly reaches equilibrium, this could be used to find critical temperature etc.
- [x] Make independent plotting function outside of simulate()