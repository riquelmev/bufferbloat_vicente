# EECS589-A1-Bufferbloat on Mininet

### Overview
In this exercise, we will study the dynamics of TCP in home networks. Specifically, we will look into a networking behavior called “Bufferbloat”. In a “typical” home network with a Home Router connected to an end host, the Home Router is connected via Cable or DSL to a Headend router at the Internet service provider’s office. We are going to study what happens when we download data from a remote server to the End Host in this home network.

In a real network, it is hard to measure CWND (as it is private to the server) and buffer occupancy (because it’s private to the router). In this assignment, we are going to emulate the network in Mininet to ease our measurement.

### Setup Instructions

Clone this strater code repo for the assignment:
```
git clone git@github.com:eecs589-advanced-networks/eecs589-a1-bufferbloat.git
cd eecs589-a1-bufferbloat
```

Run `bash setup.sh` to install the required dependencies. For more detailed steps, please refer to the assignment handout.


### Submission Instructions/Deliverables 

Please upload all of the following to canvas (using a zip file): 

* Format of the zip file: \<your uniqname>-eecs589-a1.zip

* Code: Remember one of the goals of this assignment is for you to build a system that is easy to rerun to reproduce results. Therefore, your final code MUST be runnable as a single shell command ("sudo ./run.sh"). We will test your code in the same setup.

* answers.txt: A file named answers.txt file with instructions to reproduce the results as well as the answers to the below questions. Please identify your answers with the question number, and please keep your answers brief. Please list installation instructions for any dependencies required to run your code.

* Plots: There should be 6 plots in total, 3 each for router buffer sizes 100 and 20 packets. They MUST have the following names and be present in your submission folder:
bb-q100/cwnd-iperf.png, bb-q100/q.png, bb-q100/rtt.png.
bb-q20/cwnd-iperf.png, bb-q20/q.png, bb-q20/rtt.png.



### Acknowledgments

This programming assignment is based on Prof. Changhoon Kim’s Assignment 1 from Stanford CS 244: Advanced Topics in Networking.
