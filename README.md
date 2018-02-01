# WRF_Condor
For running the WRF model in HTCondor

You should have run WPS and WRF prior to running WRF on Condor.  In this version, we're concerned with altering restart files from a 
previous WRF run.  This means that you'll have to import your wrfbdy and wrfinput files along with your restart files from the 
previous run.  WPS-specific files like met_em files should not be necessary.

Note that this will only run WRF in serial with a pre-compiled version of WRFV3.  If you want to run WRF in parallel, then you'll have to 
compile a different version of WRF and send that to the Condor sessions instead of what's already being sent from SQUID.
