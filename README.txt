Assignment details:

    Assignment 2 - Inference Engine
    COS30019 - Introduction to Artificial Intelligence
    Swinburne University of Technology
    Alex Cummaudo <1744070@student.swin.edu.au>
    Semester 1, 2016

Download executable binary in an Oracle VirtualBox VM from here:

    https://cloudstor.aarnet.edu.au/plus/index.php/s/cwR4GzwL5vRJW2b

To import the Virtual Machine, refer to the instructions here:

    https://docs.oracle.com/cd/E26217_01/E26796/html/qs-import-vm.html

To execute, navigate to the desktop and run iengine.sh with specified parameters, or --help to find usage:

    $ cd ~/Desktop/inference-engine
    $ ./iengine.sh

If the binary does not work, try recompiling by removing the bin directory:

    $ cd ~/Desktop/inference-engine 
    $ rm -rf bin
    $ ./iengine.sh

Please refer to report.pdf for further details on the implementation.

Usage:
  iengine file command
  iengine --help

Propositional logic inference engine

File:
  Expects a file whose first line TELL's the knowledge base of its
  percepts and whose second line ASK's the knowledge base a query. Ensure
  that every sentence in your knowledge base has a trailing semicolon:

    TELL
    r; !u; p & !u => w;
    ASK
    w

Command:
  [TT]  infer query from knowledge base using truth table method
  [BC]  infer query from knowledge base using backward chaining method
  [FC]  infer query from knowledge base using forward chaining method
  [RE]  infer query from knowledge base using resolution method
  [CNF] convert knowledge base and query to CNF form
  [NNF] convert knowledge base and query to NNF form
