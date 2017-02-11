# Dependencies and Libraries

## Dependency
* Note the vocabulary definition
  * Simply: My software needs other software to do its job
* Why would I depend on other software?
  * Well, more on that later
* Slight expansion on typical term
  * Dependencies are also components in the environment
    * A database or backing store
    * A web service
    * A translation service
  * Anything that your software needs outside of your code to operate
* Creates a link to functionality
* Nearly every piece of software has dependencies
  * Runtime
    * JVM
    * libc
    * interpreters
  * Runtime libraries
    * java.lang.*
    * stdio.h

## Libraries
* See definition
* A library helps do work you don't have to do
  * Defines functions you can call to do things
  * Specifies data types that you may operate on
* Reasons to use a library
  * The code already exists
  * The work needed is hard
    * Special eye on security
    * Special eye on where things can go wrong
    * Special eye on experts who have already done it
  * Excellent examples
    * [OpenSSL](https://github.com/openssl/openssl/tree/master/crypto/aes) - AES code
    * [Apache Commons HTTP client](http://svn.apache.org/viewvc/httpcomponents/oac.hc3x/trunk/src/java/org/apache/commons/httpclient/) -HTTP handling
    * [Ruby](https://github.com/ruby/ruby/blob/trunk/lib/resolv.rb) - DNS resolver
* Your program declares a need for the library
  * Java - `import com.bitnebula.ILYB`
  * Ruby - `require 'ilyb'`
  * C/C++ - `#include ilyb.h`
* It can then call functions in the library or refer to types in it
* How???
  * When the code is compiled, the compiler (or linker) creates a link to the library
  * It needs to know where to find the data
    * Example: with C, function declarations and types are in header files
  * Compilers hande this differently
    * Java: the code has a public method in a compiled class in a jar file
    * Perl: the @INC paths are searched for modules used
    * C: the -I argument includes a path to header files to find fxns
  * When found, a link is made during compilation
  * During runtime...
    * The runtime attempts to locate the compiled dependency
      * May be part of the runtime
      * May be outside the runtime, but brought in
      * Compiled languages search paths for the library
      * Interpreted languages also search paths, but execute the dependency rather than oink to it
    * Finding libraries is different per runtime
      * Java: CLASSPATH
      * C/C++: LD_LIBRARY_PATH (Linux/Solaris), LIBPATH (AIX), PATH (Windows)
      * .NET: placed in bin directory
      * Ruby: GEM_PATH
      * Perl: @INC, PERL5LIB
      * Most are environment variables
    * Now that it knows where the code is, it uses it when appropriate
* Static versus shared
  * A shared library is outside of the binary
    * Must be on the machine running the code
    * Search paths are examined when the program starts
    * Libraries can be installed in a common place
      * All programs dependent on the library use the same one
      * Permits upgrading just that library
    * Again, different formats per runtime
      * UNIX/Linux: .so file (shared object)
      * Windows: .dll file (dynamically linked library)
      * Java: .jar file (Java archive)
    * Are consumed in compiled form
    * Proprietary code is often distributed this way (binary form) so it can be used
  * A static library is compiled into the resulting executable
    * Dependencies travel with the binary
    * Does not require the library to be on the system
    * Increases the size of the binary
    * Must have the source code or the object file
* Complex applications have complex dependencies
  * Some (scary) examples:
    * [TheDailyWTF](http://thedailywtf.com/articles/The-Enterprise-Dependency)
    * [Blog post](http://technogems.blogspot.com/2011/09/dependency-graph-visualization.html)
    * [libxml by Meeting C++](https://meetingcpp.com/index.php/br/items/releasing-boost-dependency-analyzer-1-1.html)
  * Sometimes it gets out of hand
  * Dependency hell
    * Version specific links between dependencies
    * Conflicting needs
    * Example: foo
       * Depends on: libfoo v1
       * Depends on: libbar v2.3
         * Depends on: libwhatev v3.3
           * Depends on: libfoo v2.8
           * Depends on: libintl v1.1
    * Two different versions of libfoo are needed
      * Not a big deal if v2 is fully backwards compatible and the binary was not linked against the specific version
      * Otherwise... You are in bad shape

## Automated dependency management
The civilized way to deal with builds

* Remember how we said the libraries need to be there during build?
  * Where do you find them?
  * Is it safe to download and use?
* Born in the Open Source world
* Apache Ant -> Apache Maven -> Gradle
* Simplifies finding and building against dependencies
  * Maintains a registry of libraries and where to get them
  * Obtains the libraries at build time
  * Automates the build of the project
    * Build procedures are declared
    * Tasks are executed automatically
    * Non-dependent tasks can be parallelized
    * Scales to very large and complex projects
    * Incremental builds


## Vocabulary
* *Dependency* - A loose term when a piece of software relies on another piece of software to function.
* *Library* - A collection of resources used by a program to perform work. May include configuration data, documentation, help data, message templates, pre-written code and subroutines, classes, values or type specifications. Colloquially, a library usually means function definitions, routines and types in compiled form used by your program.
* *Coupling* - the degree of interdependence between software modules; a measure of how closely connected two routines or modules are; the strength of the relationships between modules.
