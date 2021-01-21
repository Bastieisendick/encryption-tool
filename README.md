# encryption-tool
Application with GUI to encrypt and decrypt files


This tool uses Caesar like encryption, BUT instead of Caesar it changes EVERY Character of the file to a random generated other character. In the end you get 3 files as output: a key file containing the Caesar numbers turned in Characters, a character list with all the possible characters used in the file and a coverted file which is all the converted chars. This is quite a cpu consuming task, so I added multiprocessing. The tool is also converted to an exe file by pyinstaller, so you can just create a shortcut and dont have to install python on your machine. The source Code is also in a zip file.
