# The Associate Hacker's Handbook - Level 3
You did it!  You finally managed to get an actual job in Security Engineering or Penetration Testing.  You've come a long way and are now learning that you still have much to learn before you can call yourself a professional.  People are impressed by your efforts and you should be proud of yourself for making this far.

You should not be in this level unless you understand the technologies, methodologies, vulnerabilities, and security solutions listed in the Newbie's Handbook.

**This portion of the series is for people who are skilled enough to get hired as a Entry Level Penetration Tester.**  The things we are going to learn about now are considered advanced and are meant to promote you from an Associate Security Consultant to an _Offical_ Security Consultant.

-------

## What you should focus on:
You've already learned a great deal about Web Applications and can effectively test them for vulnerabilities as well as discuss modern remidations to clients.  Great!  Now, it is time to level up your Reverse Engineering skills, learn low-level computation and memory management, Mobile Application Security and discover ways to bypass modern OS-Level protections such as DEP, ASLR, and Stack Canaries.

There's still a long road ahead, but you should be proud of yourself for making it this far.

### Mastering the Big 4
Below is a list that I like to call the BIG 4.  Your employer should have confidence when scheduling you on work that invovles both **attacking or code reviewing** any of the following 4 areas:
  * Network Security
  * Web Application Security
  * Binary Security / Reverse Engineering
  * Mobile Application Security
  
-------
# Table of Contents
## Advanced Penetration Testing Tools
 * **More Reverse Engineering Tools**
   * Flare VM
   * Fuzzing
     * Spike\
       * generic_chunked
       * generic_send_tcp
       * generic_send_udp
       * generic_web_server_fuzz
       * generic_web_server_fuzz2

 * **Mobile Application Hacking Tools**


## Advanced Network Security



## C/C++ Programming Essentials
 * Variable Types
   * int
   * double
   * float
   * char
 * stdin & stdout
 * File Descriptors
 * Sockets
 * Signed vs. Unsigned
   * Twos-Compliment
 * Object-Oriented Programming
   * Encapsulation
   * Abstraction
   * Inheritance
   * Polymorphism
 * Buffers
   * Arrays
   * Strings _(Behavior in memory)_
 * Pointers
   * Smart Pointers
   * Linked-Listed
 * Vectors
 * Type Casting
 * References

## Reverse Engineering
 * **Binary Fundamentals**
   * Endianness
   * The Stack
     * Stack Frames
       * Function Recursion
   * The Heap
     * Allocating Memory
     * Freeing Memory
     * Garbage Collections
   * CPU Registers
     * Intruction Pointer _(EIP / RIP)_
     * Stack Pointer _(ESP / RSP)_
     * Base Pointer _(EBP / RBP)_
 
 * **Modern Binary Protection Techniques**
   * OS-Level Protections
     * NX-Bit _(DEP)_
     * ASLR
     * CFI _(CFG & RFG)_
       * Code-Pointer Separation
       * Code-Pointer Integrity
       * Vtable Pointer Verification
   * Compile-Time Protections
     * Stack Canaries
       * Random canaries
       * Random XOR Canaries
       * Terminator Canaries
     * SafeSEH & SEHOP
       * Zeroing CPU Registers
     * Isolated Heaps _(MS14-035)_
     * Microsoft's MemoryProtection _(MS14-037)_
  
 * **Binary Hacking Techniques**
   * Stack-Based Buffer Overflow
     * Return Pointer Overwrite
     * NOP Sleds
     * Off-By-One Error
   * SEH-Based Buffer Overflow
   * Heap Exploitation
     * Use-After-Free
       * Danguling Pointers
       * Type Confusion Attacks

## Mobile Fundamentals
 * Mobile Communications
   * SIM Card
   * LTE
   * 3G
   * 4G
   * 5G
 * Mobile Data Storage
 * Rooting
 * Jailbreaking
 * APKs


## Mobile Application Security
 * **Mobile OWASP Top 10**
   * Improper Platform Usage
   * Insecure Data Storage
   * Insecure Communication
   * Insecure Authentication
   * Insufficient Cryptography
   * Insecure Authorization
   * Client Code Quality
   * Code Tampering
   * Reverse Engineering
   * Extraneous Functionality

 

## Advanced Web Application Security Bypasses
 * Bypassing Modern XSS Protections
 
