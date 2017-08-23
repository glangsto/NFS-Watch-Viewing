# NFS-Watch-Viewing
Python code for displaying raw and calibrated NSF watch (watch.py) observations

These commands produce plots of NSF_watch files._
They are installed in the Linux/Mac  bin directories, and are executed
on the terminal command line.   To work the directory ~/bin must be in your path.

To install, pull all these files into your ~/bin directory.

Then go to your data directory.  I typically keep different days data in different 
directories.

The one of the following commands:
ls      - list all files in the directory
ls *.hot  - list all the calibration files in the directory
ls *.as   - list all the astronomy files in the directory
S *.ast *.hot   - Summarize the observations in this directory
R *.ast *.hot   - Plot all the astronomy and calibration observations (only first 15 are actually plotted)
T 300.  *.hot *.ast  - Calibrate and Average the observations for 300 seconds and calibrate, plotting as many files as possible
M 300.  *.hot *.ast   - Calibrate and Average the observations, removing a baseline from a fit of data outside the normal Milky Way velocities

