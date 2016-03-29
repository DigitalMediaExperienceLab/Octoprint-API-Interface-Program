# Octoprint-API-Interface-Program
Allows access to the Octoprint API through interfaces like the command line of another computer.

 **Motivation**
 To be able to easily interact with several instances of octoprint on remote computers easily, initially through a commandline interface.
 
 **Planned Funtionality**
 The commandline program should be invoked with an option and additional arguments in the folowing ways:
 > With a -p option to print (a filename must be specified if not used with -u)
 
 > With a -u option followed by a specified local file to be uploaded to the Octoprint instance (me be combined with -p for imediate printing)
 
 > With a -d option and a filename to delete a file. specifying this with the upload function is meaningless, as it would delete the file after uploading, unless specified with the -p option which would ensue the print is prined first. (may be invoked with only the -p option, for deletion after printing)
 
 > With an -a argument at all times, to specify the API key of the target instance
 
 > With an -r option to specify th adress and port of the remote machine (ie 0.0.0.0:5000) unless the machine in question is the same as that which the command is invoked on (in which case the API may be acessed through the 'localhost' software loopback)
