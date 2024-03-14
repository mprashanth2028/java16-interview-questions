**java16-interview-questions**

**Interview Questions**

| Sno | Question                                                 | 
|-----|----------------------------------------------------------| 
|   1 |  **Java 16 -Sealed Classes**                             | 
|   2 |  **Java 16 -Pattern Matching for instanceof**            |
|   3 |  **Java 16 -Warnings for Value-Based Classes**           |
|   4 |  **Java 16 -Record**                                     |
|   5 |  **Java 16 -Packaging Tools**                            |
|   6 |  **Java 16 -Garbage Collectors**                         |
|   7 |  **Java 16 -Other Changes**                              |
|   8 |  **Java 16 -Deprecation & Removals**                     | 


**Interview Questions with Answers**

[Q1](https://github.com/mprashanth2028/java16-interview-questions?tab=readme-ov-file#Q1) **Java 16 -Sealed Classes**

sealed classes as preview feature which provides a fine grained control over inheritance

[Q2](https://github.com/mprashanth2028/java16-interview-questions?tab=readme-ov-file#Q2)**Java 16 - Pattern Matching for instanceof**

Type test pattern has a predicate to specify a type with a single binding variable

[Q3](https://github.com/mprashanth2028/java16-interview-questions?tab=readme-ov-file#Q3)**Java 16 - Warnings for Value-Based Classes**

java.util.Optional and java.time.LocalDateTime,Wrapper classes,Double class are value-based. Such Instances of a value-based class are final and immutable. Such classes have annotation @jdk.internal.ValueBased and Java 16 now generates compile time warnings in case such classes are synchronized using synchronized keyword.

[Q4](https://github.com/mprashanth2028/java16-interview-questions?tab=readme-ov-file#Q4)**Java 16 - Record**

Used to create of immutable data objects

[Q5](https://github.com/mprashanth2028/java16-interview-questions?tab=readme-ov-file#Q5)**Java 16 - Packaging Tools**

Packaging tool is developed to provide native installer for an operating system. For example, an msi/exe for windows, pkg/dmg for MacOS, deb/rpm for Linux and so on. Without this tool, developer generally share a jar file which a user has to run within own JVM.

Developer can use jlink to compress the required JDK modules to minimum modules and use the jpackage to create a lightweight image


[Q6](https://github.com/mprashanth2028/java16-interview-questions?tab=readme-ov-file#Q6)**Java 16 - Garbage Collectors**
Z Garbage Collector.ZGC is highly performant and works efficiently even in case of massive data applications e.g. machine learning applications. It ensures that there is no long pause while processing the data due to garbage collection. It supports Linux, Windows and MacOS.

With Java 16, ZGC Thread-Stack processing is moved from Safepoints to Concurrent Phase and improved its efficiency to great extent

[Q7](https://github.com/mprashanth2028/java16-interview-questions?tab=readme-ov-file#Q7)**Java 16 - Other Changes**
JEP 338 − Vector API (Incubator)
JEP, a new VECTOR API is introduced to allow developers to perform Vector operations explicitly.

JEP 347 − Enable C++14 Language Features

JEP 347, now Java formally allow C++ source code changes within the JDK to use C++14 language features,

JEP 357/369 − Migrate from Mercurial to GitHub

Large File size of version control system metadata (Mercurial)

Available tooling

Available hosting

JEP 380 − Unix-Domain Socket Channels

The Unix-domain sockets are for inter-process communication (IPC) on the same host, to exchange data between processes. 

[Q8](https://github.com/mprashanth2028/java16-interview-questions?tab=readme-ov-file#Q8)**Java 16 - Deprecation & Removals**


ThreadGroup methods like stop, destroy, isDestroyed, setDaemon and isDaemon methods are deprecated and will be removed in future release. 

Signal Chaining APIs like sigset, signal are obsolete and their use is deprecated. 
java.security.cert APIs representing DNs as Principal or String objects are deprecated.

elliptic curves which are either obsolete or not implemented using modern formulas and techniques of SunEC provider are removed.

Removals
The non-public class java.awt.PeerFixer is removed. Its purpose was to provide deserialization support of ScrollPane objects created prior JDK 1.1.1.

jaotc, an experimental Java Ahead-of-Time compilation tool is removed. Experimental Java-based JIT compiler, Graal, is also removed.

root certificates with weak 1024-bit RSA public keys have been removed from the cacerts keystore.

