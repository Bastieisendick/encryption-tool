# encryption-tool
Application with GUI to encrypt and decrypt files


This tool uses Caesar like encryption, BUT instead of Caesar it changes EVERY Character of the file to a random generated other character. In the end you get 3 files as output: a key file containing the Caesar numbers turned in Characters, a character list with all the possible characters used in the file and a coverted file which is all the converted chars. This is quite a cpu consuming task, so I added multiprocessing. The tool is converted to an exe file by pyinstaller, so that you can just create a shortcut and dont have to install python on your machine. The source Code is also in a zip file called encryption_tool_sourcecode.zip. 

To run the exe version of the encryptor unzip all and just double click on encryption_tool.exe or make a shortcut 

If you want to edit the source code by yourself, you can read yourself into bad code.

You will need to install pyinstaller
I would suggest(thats what i always did) to first:

convert your converter.py to an exe file
Do this by

pyinstaller converter.py -w 

then put all the  outputted files into the converter directory

after that you could start python encryption_tool.py or  convert it also to an exe file by:

pyinstaller encryption_tool.py --add-data tkdnd2.8;tcl -w

you will have to put the data and converter directorys inside the encryption_tool.exe directory


if you have problems how to convert to exe you can watch on my structure in the preconverted exe zip directory


The settings of the Encryptor can make the time consume better, but some break the Program, so just try out what goes the quickest for you. For me the standard works as one of the best. Also the languages should be OK to read, but not perfect.

When you want to run the code as python code, Im not shure if it will work, cause you will have to change the part with subprocess.popen to a python file. 



You will also see that theres some other files in the zip:
analyzation=  Tested my code and noted all the run times of it
set_settings.py= Can reate settings file in data directory
translate.py= is used to translate all the tkinter labels in to manyMANY languages and save them in sqlite database in data directory

these files arent really looking good code, but they work

This tool uses:

google_trans_new https://pypi.org/project/google-trans-new/
googletrans https://pypi.org/project/googletrans/

TkinterDnD2 https://github.com/pmgagne/tkinterdnd2
