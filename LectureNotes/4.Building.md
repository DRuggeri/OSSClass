# Delivering
Turns raw code into a potential product


## Overview
* Code by itself is not  useful
* It must be made useful for machines before it is useful for people
  * For compiled languages, the code must be turned into machine-readable format
    * C, Java, .net, golang
  * Interpreted languages also compile... They just do it for you just before running
    * Perl, python, ruby
  * Scripts are raw commands
    * Bash, bat, sh
* Steps to become useful (not all always apply)
  * Compiling transforms the code from human format to machine instructions
    * Requires a compiler program
    * The compiler spits out a binary format used by the runtime
    * Examples...
      * Java: JVM
      * C: libc, libcmt
      * Python: pyc
  * Packaging or bundling
    * Collect the various binaries into a useful object
    * Generally an archive
      * Native OS packages
        * RPM
        * deb
        * MSI
      * Regular archives
        * zip
        * tar
      * Runtime specific
        * jar (java archive)
        * war (java web archive)
        * apk (android package kit)
    * Dependencies
      * Let's talk about that another day...
  * Deploy it!
    * Stick it into the runtime
    * Highly dependent on what you wrote and how it gets run
    * Some examples:
      * Deploy your war file to Tomcat
      * Unzip your PHP files in docroot
      * Use yum to install your RPM on a server
      * Deploy your .net project to IIS
      * Extract the tarball of your Python scripts in /usr/local/bin
      * Use the app store to install your iPhone app
* Done! Now use it

## Demonstration
* Get the code for our sample webapp
* Build it in intelliJ
* Deploy the war file to tomcat
* Start tomcat

## CI
* That was great... but was dangerous
  * What if my computer is compromised?
  * What if I am a malicious coder?
  * What if I don't want to do all that work?
  * What if I made a mistake during the process?
  * What if all that takes me too long?
* Analysis result: humans suck!
* Enter Continuous Integration!

## Vocab
* *Compiler* - program that converts instructions from code to machine-usuable instructions
* *Runtime* - a library or program that interprets programming instructions to low level actions. Often greatly simplifies the work for the programmer