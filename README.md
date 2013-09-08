makeh2kit
=========

BASH script to auto-generate .h2drumkit files

Running 'makeh2kit' with no arguments scans the current directory for .flac files and creates a .h2drumkit file named after the current directory. Instruments are named after the audio files minus the extension.

FLAC, WAV, AU, or AIFF files can be scanned for, e.g.

    makeh2kit -f=wav

The drum kit name, author, license, and info can also be specified on the command line. When supplying arguments to these options use single rather than double quotes to allow for use of special characters. In addition, HTML formatting tags can be used with the --htmlinfo option:

    makeh2kit --hi '<p><b>Kit Name</b></p><p>Kit description</p>'

For a full list of options, run:

    makeh2kit -h

Once downloaded, make the script executable (e.g. right click the file and select Properties->Permissions) then copy to /usr/bin with:

    su -c 'cp makeh2kit /usr/bin'

or

    sudo cp makeh2kit /usr/bin
