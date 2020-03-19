# MiniProject_Face_Similarity

A face similarity finder that has a front end web application with PHP at backend and uses python at server to find similarity between two faces given as input. The two faces shall be, 
  1. from documents
  2. one clicked from webcam and other from produced documents
 
Application:

  Use of this application at exam centers for verification of students can reduce potential threat of cheating and forgery by means of candidate replacements. 

Requirements:

  1.XAMPP or any PHP server.
  
  2.Python v3.6.
  
  3.Packages for python are listed in packages.txt.
  
  4.If using windows, a C/C++ compiler (MSVC preferred with Visual Studio 2012 and above).
  
While installing packages in windows, do from cmd prompt opened in with admin priveleges.

Troubleshooting:
  1. Error : NO_C_COMPILER FOUND or NO_CXX_COMPILER FOUND
    This means that your cmake was not able to identify or access C/C++ compiler in your system. 
    Steps to resolve:
      (i) Make sure a C/C++ compiler is availabe in your system. If you are using MSVC, make sure it has downloaded the necessary C/C++ workspace. If using GCC or MinGW, make sure it is installed properly by checking for its version with "gcc --version" in cmd prompt.
      
      (ii)If still the error persists, manually open Cmake GUI in this path,    
      "C:\Users\<YOUR_USERNAME>\AppData\Local\Programs\Python\Python36\Lib\site-packages\cmake\data\bin\cmake-gui.exe",
      open it, click configure and manually set path of C_COMPILER and CXX_COMPILER to your installed C/C++ compiler respectively.
      Then delete cmakecache in the same folder and configure a new sample cmakelists.txt file, with following contents just to test,
          
    project ("CMakeProject3")
    add_subdirectory ("CMakeProject3")
    
    And then click generate in GUI.
    
    (iii) Make sure cmake is installed via cmd prompt opened in admin priveleges.

Procedure: (If using xampp server)
  1. Install the requirements stated.
  2. Clone this repository and extract all files into C:/xampp/htdocs.
  3. Goto browser and navigate to localhost/snapper.php.
  4. Make sure webcam access permission is given to localhost in your browser.
