# EPU_eucentric_workaround

This script provides a workaround for when EPU will not move from the center of a grid square and the user needs to manually set eucentric height. To use, move elsewhere in the grid square, do "auto-eucentric by beam tilt" in EPU (_not_ the automated one in the EPU workflow) and note the eucentric height. Then, navigate in the terminal to your current EPU folder on the support PC and run the script (in a bash environment -- I recommend WSL Ubuntu) while inputting the GridSquare number and eucentric height manually:

```
bash /path/to/script/eucentriccorrection.sh {gridsquare} {eucentric}
```
```
bash /path/to/script/eucentriccorrection.sh 12345678 40.00
```

The gridsquare number can be determined by looking (usually) at the most recently updated folder in Images-Disc1, especially if you re-take the grid square image before running. 

You may need sudo privileges to run the script. If requested, add "sudo" before "bash" in the above command. 
