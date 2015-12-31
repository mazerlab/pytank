python/shell based tank extraction tools
----------------------------------------
getexpers.sh*			generate list of exper from data directories
exper2hdf5.sh*			convert tanks for entire 'exper' 
tank2hdf5.py*			convert tanks each pypefile on command line

Example usage:

    % getexpers /auto/data/critters/bert/2015/2015-05* | xargs -n1 exper2hdf5

This will generate HDF5 versions of the tdt DataTanks for all
experiments found in May 2015. It'll take a while to run, but the fast
loading speed of the HDF5 files makes it worth the time.

matlab tank tools
------------------------------
th5dump.m				pointer to where the hdf5 files are cached (global)
list_tdtblocks.m		get list of tdt block names from pypefiles
loadall.m				load all tank data associated with an 'exper'
showsnips.m				make plot of randomly selected subset of snips






