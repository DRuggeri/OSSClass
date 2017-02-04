# Delivering
* Turns raw code into a potential product
* Demonstration to drive home the point that this is a _process_
  * Download software
  * Unpack it
  * ./configure --blah
  * make
  * make install


## Overview
* Code by itself is not useful
* It must be made useful for machines before it is useful for people
  * For compiled languages, the code must be turned into machine-readable format
    * C, Java, .net, golang
  * Interpreted languages also compile... They just do it for you just before running
    * Perl, python, ruby
  * Scripts are raw commands
    * Bash, bat, sh
* Steps to become useful (not all always apply)
  * *Compiling* - transforms the code from human format to machine instructions
    * Requires a compiler program
    * The compiler spits out a binary format used by the runtime
    * Examples...
      * Java: JVM
      * C: libc, libcmt
      * Python: pyc
    * Let's see it in action...
      * Commence the compiling demonstration below
  * *Packaging* or bundling gets the compiled code to a deployable _thing_
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
    * Stick it into an environment
      * See environment definition below
      * See runtime definition below
    * Highly dependent on what you wrote and how it gets run
    * Some examples:
      * Deploy your war file to Tomcat
      * Unzip your PHP files in docroot
      * Use yum to install your RPM on a server
      * Deploy your .net project to IIS
      * Extract the tarball of your Python scripts in /usr/local/bin
      * Use the app store to install your iPhone app
* Done! Now use it

## Demonstrations
* Compiling from command line
  * teh codez in hello.c
    ```
    #include<stdio.h>

    main()
    {
        printf("Hello World");
    }
    ```
  * Examine...
    * `file hello.c` - What is hello.c?
      * The file command tells us what Linux thinks this file is
      * Uses magic ([no, really... it's magic](https://en.wikipedia.org/wiki/List_of_file_signatures))
    * `gcc hello.c -o hello` - Compile it
      * Text to machine code
      * `-o hello` says to write the binary to the file "hello"
    * `ls -l` - There's a new file here...
    * `file hello` - What is hello?
    * `cat hello` - Well that sure isn't text...
    * `strings hello` - Runtime library _stuff_ added to our program
    * `./hello` - BEHOLD!!! The world has been greeted
* Compiling with NetBeans
  * File -> New project
    * Java -> Java Application
    * Project Name -> HelloWorld
  * teh codez in HelloWorld.java
    ```
    package helloworld;

    public class HelloWorld {
        public static void main(String[] args) {
            System.out.println("Hello World");
        }
    }
    ```
  * Save the file and click the green run button
  * BEHOLD!!! The world has been greeted

## Vocabulary
* *Compiler* - program that converts instructions from code to machine-usuable instructions
* *Runtime* - a library or program that interprets programming instructions to low level actions. Often greatly simplifies the work for the programmer.
* *Environment* - a collection of local (to the software) configurations, external services (databases, webservices, etc) and the runtime that  serve as a delivery point for the software. Environments typically serve a specific purpose such as development, testing, production and disaster recovery.
* *Package/Artifact* - the product of a software build procedure. Typically an archive or collection of the compiled software in a near-ready to ship state.
