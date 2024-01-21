#------- Alan Alarcón SAC tutorial
#	a.alarcon@igeofisica.unam.mx
#
#	SAC 101.6a
#	SEISMIC ANALYSIS CODE [06/12/2013 (Version 101.6)]
#	Copyright 1995 Regents of the University of California
#
#	SAC INSTALLATION PROVED ON UBUNTU 20.04, 22.04
#	LAST UPDATE 21/01/2024
#	Check and/or download the manual 
#
#	http://ds.iris.edu/files/sac-manual/
#	 
#	Recomendation
#	
#	1. Install gedit
#	open a terminal ( Ctrl + T ) and paste:
#	sudo apt-get update 
#	sudo apt-get install gedit
#	Close the first terminal and opened again
#
#	2. Make a "programs" directory
#	open a terminal ( Ctrl + T ) and tape:
#	mkdir programs
#	cd programs
#	mkdir SAC
#
#	SAC installation:
#	
#	1. Go to directory where you put the file extraction
#	/home/your user name/programs/SAC/bin
#	
#	2. Looking for "sacinit.sh" file and edit the 18th line with
#	/home/put your username/programs/SAC/
#
#	3. Save and close teh gedit window
#
#	4. Now, we are going to add some lines in the .bashrc file so, first of all, open a terminal ( Ctrl + T ) 
#	
#	5. Tape gedit .bashrc 
#
#	6. Go to the end (be careful) and paste the next lines:

##################	SAC	####################
export SACHOME=/home/put your username/programs/SAC
export PATH=${SACHOME}/bin:${PATH}
export LD_LIBRARY_PATH=${LD_LIBRARY_PATH}:${SACHOME}/lib
export C_INCLUDE_PATH=$C_INCLUDE_PATH:${SACHOME}/include
export SACAUX=$SACHOME/aux
alias sac="$SACHOME/bin/sac $SACHOME/macros/sac.init"

#	7. Save the file and close the window :)
#
#	8. Back into the terminal and tape:
#	source .bashrc
#	
#	9. For any doubt xddd, close the old terminal and open another terminal and tape:
#	SAC
#	***If works, you can read a message like:
 SEISMIC ANALYSIS CODE [06/12/2013 (Version 101.6)]
 Copyright 1995 Regents of the University of California

SAC> 
#	All done :)



