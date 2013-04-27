This script is written by Mark Jenkins of FMRIB http://users.fmrib.ox.ac.uk/~mark/ 
He posted it on the FSL mailing list at some point but I could not find it anywhere else. 
All credit should go to him I only share it here so others can find it easier.

These are his instructions:
=========================================
"I've previously written a little script to do this which I'm including below. The displacements are always relative to the first timepoint (assuming the reference_no of 0 was used in eddy_correct) but apart from that it is pretty general.

If you run it you just need to give it the name of the .ecclog file (it also assumes the original data has the same - without the .ecclog extension). It will then produce ec_disp.png, ec_rot.png and ec_trans.png images and the associated .txt files with the numbers in them.

Let me know if you have any trouble running it. You should just need to copy the text below into a file (make sure you keep it as pure text and don't use Word or anything like that to make the file) called ec_plot.sh and then do :
 chmod 755 ec_plot.sh
If you put it in $FSLDIR/bin/ then it will be available wherever you are, but if you put it somewhere else then you'll need to specify the path before the "ec_plot.sh" name when you run it  (e.g.   ~/scripts/ec_plot.sh myfile.ecclog if you put the file in ~/scripts/ )

All the best,
       Mark 
=======================================
original posting https://www.jiscmail.ac.uk/cgi-bin/webadmin?A2=FSL;b864bc43.1101