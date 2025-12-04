# Reliable-set-tools-in-Python-Software-for-the-analysis-of-seismic-volcanic-signals

A reliable Python software toolkit for seismic-volcanic signal analysis, featuring a GUI that facilitates efficient management of seismic signal formats. It offers fast and easy management of analysis time and generates conclusions that provide further information about volcanic processes (pre-eruptive and post-eruptive).

Version 1.1
-------------------------------------------------------------------------------------------------------------------------------------------
          Theoretical Physics and the Cosmos Department
      Signal Theory, Telematics and Communications Department
---- Andalusian Institute of Geophysics and Prevention of Seismic Disasters ----------
      Granada University (Ugr), Granada, Spain
-------------------------------------------------------------------------------------------------------------------------------------------

    Author: Developed, Design and writing by: Ligdamis A. Gutiérrez E. PhD. (1,2)
    Granada, Spain 2021-2023

Institutions associated:

(1) Department of Theoretical Physics and Cosmos. Science Faculty. Avd. Fuentenueva s/n. University of Granada. 18071. Granada. Spain.

(2) Andalusian Institute of Geophysiscs. Campus de Cartuja. University of Granada. C/Profesor Clavera 12. 18071. Granada. Spain.

'' WARNING: Do not modify or edit the code without permission of the author.
    In case of using this software, indicate and refer to the author and the institution he represents.
    The University of Granada, Ugr ''

-------------------------------------------------------------------------------------------------------------------------------------------

Acknowledgment:

This software is the product of the research by the Spanish projects:

a)    PID2022-143083NB-I00, “LEARNING”, funded by MCIN/AEI /10.13039/501100011033
b)    JMI and LG were partially funded by the Spanish project PROOF-FOREVER (EUR2022.134044)
c)    PRD was funded by the Ministerio de Ciencia e Innovación del Gobierno de España (MCIN), Agencia Estatal de Investigación (AEI), Fondo Social Europeo (FSE), and Programa Estatal de Promoción del Talento y su Empleabilidad en I+D+I Ayudas para contratos predoctorales para la formación de doctores 2020 (PRE2020-092719).
d)    Spanish Project PID2022-143083NB-100 founded by MCIN/AEI/10.13039/501100011033 and by FEDER (EU) “Una manera de hacer Europa”.
e)    PLEC2022-009271"DigiVolCan”, funded by MCIN/AEI, funded by MCIN/AEI/10.13039/501100011033 and by EU «NextGenerationEU/PRTR», 10.13039/501100011033.

-------------------------------------------------------------------------------------------------------------------------------------------

Introduction:

Dear User:

This file contains information related to the Application.
Please read it carefully before starting work.

In the same way, it is recommended to review the contents of the manual attached to the documents, in order to become familiar with the different actions that can be carried 
out, through the elements of system management.

The system was developed in version 3.8.6. of the Python language.
The software is open source and can be downloaded from the website:

https://www.python.org/downloads/release/python-386/

***(However, it can operate without problems in Python, version 10.10)***

Since Python a multiplatform lenguaje, it works the same on Windows, Linux, Mac systems, or Android for Tablets and mobile phones (after adapting Python for these devices).

It works on 32 and 64 Bit Systems (x86, win64), under Windows (7, 8, 10, 11).
This Software has been tested on Linux systems on Ubuntu 20 and the macOS for Mac System.
Additionally, should work without problems in other similar Linux systems like: Debian, Ret Hat, Fedora, SUSE, etc.

The version of Python in which the interface has been programmed is 3.8.6. However, it can operate without problems in Python, version 10.10
Any modification of the Python codes in a different version can be cause alterations in the functioning of the system.
The Python documentation must be revised to adapt the code to the correct version.

For the reading and manipulation of common file formats, access data centers and seismological signal processing routines the "ObsPy" library is used. 
ObsPy is a Python framework for Seismology, is an open-source. The documentation can be downloaded from the website:

https://docs.obspy.org/

To represent the graphs, the "Matplotlib" library is used. The documentation and terms of the use of the license of the Matplotlib by the user
can be read and downloaded from the website:

https://matplotlib.org/stable/users/index.html

All main program interfaces and the text within them are designed exclusively in English. However, the user manual is written in both English and Spanish. 
The documentation, or "user manuals," are available as PDF files, organized into two folders: "a) Document_EN" and "b) Document_ES," 
written in English and Spanish respectively. These are described below:.

a) The "Document_EN" folder contains the user manuals for the 10 modules in PDF format in English. - English version

	1_Manual_Analysis_System_EN.pdf
	2_Manual_Sta_Lta_trigger_methods_EN.pdf
	3_Manual_One_Day_Records_EN.pdf
	4_Manual_Seismic_signals_converting_Wav_file_EN.pdf
	5_Manual_Seismic Signals Integration System_EN.pdf
	6_Manual_Cut_Save_Signals_Events_EN.pdf
	7_Manual_Merge_Signals_Events_EN.pdf
	8_Manual_Save_record_MSEED_and_SAC_EN.pdf
	9_Manual_Download_Records_FDSN_EN.pdf
	10_Manual_Individual Seismic Data Download FDSN_EN.pdf

b) The "Document_ES" folder contains the user manuals for the 10 modules in PDF format in Spanish - Spanish version

	1_Manual_Analysis_System_Vrs_1.pdf
	2_Manual_Sta_Lta_trigger_methods_Vrs_1.pdf
	3_Manual_One_Day_Records_Vrs_1.pdf
	4_Manual_Seismic_signals_converting_Wav_file_Vrs_1.pdf
	5_Manual_Seismic Signals Integration System_Vrs_1.pdf
	6_Manual_Cut_Save_Signals_Events_Vrs_1.pdf
	7_Manual_Merge_Signals_Events_Vrs_1.pdf
	8_Manual_Save_record_MSEED_and_SAC_Vrs_1.pdf
	9_Manual_Download_Records_FDSN_Vers_1.pdf
	10_Manual_Individual Seismic Data Download FDSN_Vers_1.pdf

Each of the user manuals contains a complete description of the objectives, use and mathematical tools for spectral analysis 
of signals for the reading, processing and results of the more general investigation of seismic-volcanic signals, 
used in observatories and research institutes. Users are advised to read the manuals provided here beforehand 
to get the most out of their work with seismic signals.


**** IMPORTANT NOTE: ****

It's recommended to have at least 8 GB or more (16 GB would be perfect) of memory in the system.

This software is the product of improvements made to version 1.0 of the previously released individual modules. 
The final result is the combination of the 10 individual modules, forming the system now presented. 
This new version includes improvements to the code and interface of each module, applying updates to both.

-------------------------------------------------------------------------------------------------------------------------------------------
GENERAL CONTENT INDEX
-------------------------------------------------------------------------------------------------------------------------------------------
1.- Main system objective.
2.- General structure and folders organization.
3.- Description of the Folders and elements containing.
4.- Prerequisites (installing Python and Pip on windows)
5.- System installation and running under windows
6.- System installation and running under Linux and Mac System
7.- Installation comments.
8.- Modules under construction.

-------------------------------------------------------------------------------------------------------------------------------------------
1.- MAIN OBJECTIVE OF THE SYSTEM
-------------------------------------------------------------------------------------------------------------------------------------------

The "Reliable set tools in Python Software for the analysis of seismic-volcanic signals" is a user-friendly interface that 
enables easy and efficient management for working with the most commonly used seismic signal formats in observatories, such as: SEISAN, GSE2, EVT, GCF, WAV, MSEED, and SAC, among others.

This entire procedure is a great practical help to some observatories that need specific tools, programs, and software to read various formats, perform calculations, 
and present results. However, they face problems due to the complexity of these tools (learning, operation, management, and modification).

Furthermore, data acquisition is carried out through external sites that the operators do not manage or control, or the data is provided 
by other observatories whose operating formats differ from those that will be processed and analyzed at the receiving observatory.

For these main reasons, it is important and extremely useful for the human operator to have an intuitive system that performs the calculation 
of large volumes of data using mathematical parameters and data input in a simple and efficient manner, obtaining more reliable and straightforward 
results at a much lower computational cost than other tools currently on the market. This allows for much better management of analysis time 
and the drawing of conclusions that provide significantly more information about volcanic processes (pre-eruptive and post-eruptive), contributing 
to the development of improved real-time early warning systems
   
-------------------------------------------------------------------------------------------------------------------------------------------
2.- GENERAL STRUCTURE AND ORGANIZATION OF FOLDERS
-------------------------------------------------------------------------------------------------------------------------------------------

The system consists of three folders with the programs (codes and interfaces in English and documentation in Spanish and English), organized as follows:

a) One Folder “Reliable_set_tools_system_1”: (seismic analysis system assembly). This folder must be copied to “My Documents”. Contains the following elements:

	I.- Subfolder: “Images” ” Images necessary for program interfaces.
	II.- Program: Menu.py. Startup program, presentation and calling of individual modules.
	III.- Ten modules composed of Python programs (.py). These main programs are designed using a GUI ("Graphical User Interface"). Each module's name and description are as follows :

		1.- "Analysis_System_1.py". Main program for spectral analysis and filtering (Lowpass, Highpass, Bandpass, and Bandstop). The types of spectral analyses avaible are:
                     	a) Fourier Transform Spectrum in the Frequency Domain.  
			b) Spectrogram using the Fast Fourier Transform (FFT).  
			c) Spectrogram with an included band-pass filter.  
			d) Envelope of the signal filtered by a low-pass filter.  
			e) Power spectral density using Welch's method.  
			f) Classical periodogram plus 5 Welch types.  
			g) Continuous Wavelet Transform (CWT) of the record.  
			h) Analysis of the Discrete Wavelet Transform Coefficients.

	 	2.- “Sta_Lta_trigger_methods.py”. Main program (interface), for the analysis of seismic records, using the both trigering methods (Recursive and classical) 
                    of the STA/LTA algorithm, with and without filter (Lowpass, Highpass, Bandpass, and Bandstop). Using two STA/LTA triggering methods: “recursive” and “classic or typical”: 
		3.- “Days_1.py”. Main program (interface), for the analysis and management of presenting complete 24-hour records in one-hour duration segments.
		4.- “Sound_1.py”. Main analysis program to select and transform seismic records into sounds in 'Wav' format.
		5.- “Integrals_1.py”. Main program for analysis and integration of seismic-volcanic events.
		6.- “Cut_1.py”. Main analysis program with filters, for cutting events within a seismic record.
		7.- “Merge_1.py”. Main analysis program for selecting and merging or concatenating a seismic event present in two separate records, in order to construct a single record for analysis
		8.- “Convert_1.py”. Main program (interface) for recording and converting seismic records in other formats to MSEED and SAC formats.
		9.- “Download_FDSN_1.py”. Main program and interface for downloading seismic records and stations from the FDSN (Federation of Digital Seismograph Networks) network.
                    Using two available domain methods: the circular domain method and the rectangular domain method and converting them into MSEED and SAC formats.
		10.- “ModIris_2.py”. Main program (interface) for searching and downloading seismic records from the FDSN network and converting them into MSEED and SAC formats.

	IV.- “Initials Requirements.txt” file. File containing the libraries needed to be installed on Windows through “Pip”, once Python is installed.
         V.- File “Set_tools_System_1_1.bat”, batch processing executable file. It must be copied to the desktop, from there by right clicking “run as administrator”, 
             it will start the system by calling the main menu. The file will automatically search for the startup program (Menu.py) that is located in the “Set_tools_System_1_1” folder 
             that has been previously copied to “My Documents” and will start Python, executing said program.

b) Two Folders (Document_ES and Document_EN, depending on the language; English or Spanish). For English “Document_EN”: It consists of the following items:

     1.- Document folder: "Document_EN" folder contains the user manuals for the 10 modules in PDF format in English. - English version 
          	1_Manual_Analysis_System_EN.pdf
		2_Manual_Sta_Lta_trigger_methods_EN.pdf
		3_Manual_One_Day_Records_EN.pdf
		4_Manual_Seismic_signals_converting_Wav_file_EN.pdf
		5_Manual_Seismic Signals Integration System_EN.pdf
		6_Manual_Cut_Save_Signals_Events_EN.pdf
		7_Manual_Merge_Signals_Events_EN.pdf
		8_Manual_Save_record_MSEED_and_SAC_EN.pdf
		9_Manual_Download_Records_FDSN_EN.pdf
		10_Manual_Individual Seismic Data Download FDSN_EN.pdf
     2.- Document folder: "Document_ES" folder contains the user manuals for the 10 modules in PDF format in Spanish - Spanish version
           	1_Manual_Analysis_System_Vrs_1.pdf
		2_Manual_Sta_Lta_trigger_methods_Vrs_1.pdf
		3_Manual_One_Day_Records_Vrs_1.pdf
		4_Manual_Seismic_signals_converting_Wav_file_Vrs_1.pdf
		5_Manual_Seismic Signals Integration System_Vrs_1.pdf
		6_Manual_Cut_Save_Signals_Events_Vrs_1.pdf
		7_Manual_Merge_Signals_Events_Vrs_1.pdf
		8_Manual_Save_record_MSEED_and_SAC_Vrs_1.pdf
		9_Manual_Download_Records_FDSN_Vers_1.pdf
		10_Manual_Individual Seismic Data Download FDSN_Vers_1.pdf
    
-------------------------------------------------------------------------------------------------------------------------------------------
3.- DESCRIPTION OF THE FOLDERS AND ELEMENTS CONTAINNING
-------------------------------------------------------------------------------------------------------------------------------------------

- In the main part there are the necessary programs for the operation of the Volcano-Seismic signals entropy analysis system. Located in the two compressed folders.
- The content is as follows:

1) Document folder

   a) The 10 user manuals (PDF). System user manuals, written in English and Spanish.
       It contains the necessary instructions for handling the system and the elements that make it up.
   b) The file README.txt. Contains the basic instructions for installing the software and all items
        that make up the system
   c) The file "Initial_requeriments.txt" contains the list of necessary libraries that python uses to run this system.
       It is recommended to execute each line in a console or "CMD" window, for the installation of the libraries                  
       through "Pip", after installing Python.
   d) The ".bat" file (Set_tools_System_1_1.bat), that facilitate the start of the system in Windows System.
        These files present a Welcome screen change to the working directory
        where the programs are located and run python with the startup program: "Menu.py" to start the system.         
        
2) Reliable_set_tools_system_1 folder

   a) "Menu.py" Program of the interface. Welcome and start the system. This interface contains the command buttons that give access to the ten modules of which the system is composed. It also allows the exit.
   b)  Programs or user interface, composed of the ten modules described in the previous point.
   c) "Images" folder, which contains the icons and images of the interfaces. It must be located in the same place as the all interface programs. This is in the "My Documents" folder.             
        
** At future, this Software may be expanded by adding new modules, containing other analysis tools, and volcano-Seismic signals classification. **
    
-------------------------------------------------------------------------------------------------------------------------------------------
4.- PREREQUISITES (INSTALLING PYTHON AND PIP ON WINDOWS)
-------------------------------------------------------------------------------------------------------------------------------------------

It's recommended to have at least 8 GB or more (16 GB would be perfect) of memory in the system.

Python and its package manager (Pip) are native to Linux languages. That is, when Linux is installed, both the Python language and its package manager (Pip) are installed. 
Although it is always recommended to have the most up-to-date version, both of Python and pip. what in Linux is done almost automatically with the application manager and that, in addition, Linux generally communicates to the user.

In the Windows system, it must be installed before using the system. Because the system itself has been created with this language. The good thing is that Python can run without problems on Windows operating systems.

There is an easy way to do this.

a) Download the appropriate version from the Python distribution web page, located at the following web address:
             https://www.python.org/downloads/

    On the Web, the correct version must be selected, according to the type of operating system
    that is in the computer, including if it is 32 or 64 bits.

    On the Web, both the executable version (.exe) and the compressed file version (.zip) or (.tz) for Linux are available for download.

Once this version is downloaded, it is installed in the operating system (as administrator). When starting the installation, a screen of the installation assistant is presented, which indicates the steps to follow to install the language.

You just have to follow the steps. It is important to leave the box to add to the windows "path" the installation path where the Python files are located. If you skip this step, you have to do this manually. Because if it is not set, Python is not recognized by the system to run.

Manually, this can also be set from the system environment variables. Manually found in: Control Panel/System/Advanced System Settings/Environment Variables/Edit

Here you set where the Python scripts and programs are located on the system. But the easiest and most prudent thing to do is to simply check the box that allows this during the Python installation.

Once Python and pip are installed on the system, check that they work. To do this, you just have to see this in a windows command window (CMD), using the following commands.

> python –V

And to verify the “pip” the following command is typed:

> pip –V

After typing “pip – V”, it is usually seen that the version of pip is “20.2.1”. At this point, it is recommended to update that version, since by default "pip" is installed together with "Python", 
but it does not install the latest or most updated version. To do this, in the CMD window or console, type the following command in: (Windows/Linux).

     Windows: > python –m pip install –upgrade pip    |   Linux: $ sudo python3 –m pip install –upgrade pip

This indicates that the "pip" will be updated to its latest version (In Linux, as "superuser", that is, "sudo" at startup). Note that for Windows, you type "python", but on Linux you must type "python3".

Once Python is installed and the "pip" is updated, you must proceed to install the additional packages and libraries that Python needs to run the system. This is done using the "pip". To do this, the file "Initial_requeriments.txt" is used, which is found with supplied files.

Proceed in the console or command window "Cmd" to install each recommended library.

Once this is done, the operating system is ready to run both python and the main program.

-------------------------------------------------------------------------------------------------------------------------------------------
5.- SYSTEM INSTALLATION AND RUNNING UNDER WINDOWS
-------------------------------------------------------------------------------------------------------------------------------------------

After downloading the items and once both the Python and the necessary additional libraries have been installed.

To install the system on Windows systems (either 32 or 64 bits), do the following:

a)  Copy the (all) folder containing the Python and data files.
     This is according to the "English" version 1.1
     Path to "Documents\Document_EN\"
     Remember, these folders (Document_EN and Document_ES), should be copied to "My Documents" on the computer.

b) Copy the ".bat" file (Set_tools_System_1_1.bat), to the desktop of the computer.

c) In the desktop, run this file as "administrator" (right click on the file and choose this option)
     The Welcome screen will be displayed:

---------------------------------------------------------------------------------------------------------

                 =================================================
             	=                                               =
             	=      Welcome to:                              =
             	=                                               =
             	=  Reliable set tools in Python Software for    =
 		=  the analysis of seismic-volcanic signals     =
                =                                               =
                =  Theoretical and Cosmos Physics Department.   = 
                =                Science Faculty                =
             	=      Andalusian Institute of Geophysics       =
             	=            Granada University (Ugr)           =
             	=                                               =
             	=          Developed in Python 3.8.6            =
             	=     Execution for Windows and Linux System    =
             	=                 2021 -2023                    =
             	=================================================

           Please, Minimize the CMD from the Python.exe window (in black).
               (Don't close it, because the system also closes).           
           When you exit the system, this window closes automatically.
           
                       To continue, please press a key.

                  *** Please, press a key to Start the System. ***

----------------------------------------------------------------------------------------------------------   
    
Pressing any key will present two screens. One in black, which is the Python command window (cmd).
This must be minimized, so that it does not disturb the view of the system.

The start and welcome screen of the "Menu.py" system will be presented. This screen is the presentation and entry to the system.
You can exit here by clicking the "Exit" button or continue by clicking any of the three available command buttons (one for each module in the system).

Clicking the command button of the selected module presents the main interface of that module.

This will display the main screen of the Main Menu interface. Here, the process actions are performed: loading each module, from which seismic-volcanic 
records are read, filter analysis, mathematical calculations and spectral analysis, saving of resulting files, etc.

The resulting graphs are also displayed. Refer to the user manual included in the documentation for each module..

To return to the main menu from an interface, click the "Back" button of each module. This action will close the current interface screen and open the main menu module again, to select a different module.

To exit, click the "Exit" button. In the dialog window, type "Ok" to accept the output. Otherwise "Cancel" to continue in the system.

-------------------------------------------------------------------------------------------------------------------------------------------
6.- SYSTEM INSTALLATION AND RUNNING UNDER LINUX
-------------------------------------------------------------------------------------------------------------------------------------------

Installation on Linux systems is similar to Windows. The main folder is copied either to the desktop, or to the personal folder, etc.

This is according to the "English" version 1.1
    Path to "Documents\Reliable_set_tools_system_1\"

From that location (inside the main folder, where the "Menu.py", 10 programs , Images folders are located), open a window or command console and type:

“$ python3 Menu.py”

This command is to start the system and proceed to perform the analysis normally.
The output is similar to Windows System, must be clicking in the "Exit" button.

Remember:
Once Python is installed and the "pip" is updated, you must proceed to install the additional packages and libraries that Python needs to run the system. 
This is done using the "pip". To do this, the file "Initial_requeriments.txt" is used, which is found with supplied files.

-------------------------------------------------------------------------------------------------------------------------------------------
7.- INSTALLATION COMMENTS
-------------------------------------------------------------------------------------------------------------------------------------------

The system works fine on Windows (XP, 7, 8, 10, 11) 32-bit and 64-bit systems.

The system it’s designed to work in multiplatform.
It is allowed by programming in Python 3.8.6. On Windows, Linux and Mac systems without problems.

Warning: Other higher versions of Python may cause problems in some libraries, check their manual to ensure proper operation.
         However, it can operate without problems in Python, version 10.10

---------------------------------------------------------------------------------------------------------------------------------------------

Warning: It is recommended not to make alterations, changes, or eliminations of part or the complete content of the codes and programs that comprise the system, 
without the necessary knowledge, since it can seriously affect its operation.

-------------------------------------------------------------------------------------------------------------------------------------------
8.- MODULES UNDER CONSTRUCTION
-------------------------------------------------------------------------------------------------------------------------------------------

Soon, in a new version or update of the current version (1.2), extra algorithms may be added, containing several types of analysis, functionalities or more methods, 
other analysis tools, and volcano-Seismic signals classification which provide an improvement in the study and research of the scientific community.


** THEY WILL BE AVAILABLE FOR DOWNLOAD IN THE FUTURE **
Thanks.
Author: Developed, Design and writing by: Ligdamis A. Gutiérrez E. PhD.
