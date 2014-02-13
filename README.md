CMSNotes
========

- get the "utils" package for standard CMS notes/papers from svn:
svn co -N svn+ssh://svn.cern.ch/reps/tdr2 myDir
cd myDir 
svn update utils

- get this package from git:
git clone https://github.com/amagnan/CMSNotes.git

- Setup environment to build with TDR style:
cd CMSNotes/
ln -s ../utils/trunk/tdr tdr
ln -s ../utils/trunk/general general
cd ../
eval `./CMSNotes/tdr runtime -sh`

- Compile with tdr style:
cd CMSNotes/PFCalEE
tdr --noclean --style=an b PFCalEE

