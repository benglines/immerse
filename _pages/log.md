---
layout: default
title: IMMERSE Log
---

## Schedule

* **Monday**:
  * 8:00am-12:00pm, 1:00pm-4:00pm
* **Tuesday**: 
  * 8:00am-12:00pm, 1:00pm-4:00pm
* **Wednesday**: 
  * 8:00am-12:00pm, 1:00pm-4:00pm
* **Thursday**: 
  * 8:00am-12:00pm, 1:00pm-4:00pm
* **Friday**: 
  * 8:00am-12:00pm

## Log

### Week 8: 14 JUNE 2021

#### Goals

* Basic SCC Decomposition Algorithm.
* Highest Fanout SCC Decomposition Algorithm
* Read paper about PIPs

#### Daily Updates

* **Monday**:
  * 
* **Tuesday**: 
  * 
* **Wednesday**: 
  * 
* **Thursday**: 
  * 
* **Friday**:
  *

### Week 7: 7 JUNE 2021

#### Goals

* Deepdive into SpyDrNet SHREC API so I can start implementing new algorithms and features
* Work on SpyDrNet SHREC "Voters Before/After Every Flip-Flop" algorithm
* Clean up/add to bit2fasm module on Computing Boot Camp page, and also make a pull request for the rest of the changes I've made. 
* Read "Synchronization Techniques for Crossing Multiple Clock Domains in FPGA-Based TMR Circuits" to learn more about clock domains.
* Work with Jacob on SpyDrNet SHREC tutorial page.
* Basic SCC Decomposition Algorithm
* Black box voters

#### Daily Updates

* **Monday**:
  * Finished reading TMR paper.
  * Started implementing voter after every flip-flop.
* **Tuesday**: 
  * Finished voter after every flip-flop algorithm. 
  * Also finished voter before every flip-flop algorithm. This one took a bit of time, but I got it working as far as I can tell. I want to create some tests for both of these algorithms to ensure they are working properly. 
* **Wednesday**: 
  * Turns out the algorithm for placing a voter before every flip-flop wasn't working after some more testing. Worked on redo-ing it to make it work.
  * Added documentation for both algorithms
* **Thursday**: 
  * Fixed placing voter after every flip-flop algorithm. As far as I can tell, it seems to be working well.
  * Finalized documentation and style fixes for both algorithm
  * Created example that demonstrates using both algorithms
* **Friday**:
  *

### Week 6: 31 MAY 2021

#### Goals

* Get SpyDrNet SHREC tests working, and add a couple tests.
* SpyDrNet SHREC examples:
  * Reduction vs. feedback voter example (example with replicated ports, and an example with the orignal ports)
  * Inoutput port example
  * Bigger design, perhaps my RISCV processor from 323.
* Finish making tutorial page for SpyDrNet SHREC
* Finish reading TMR paper.
* Read "Synchronization Techniques for Crossing Multiple Clock Domains in FPGA-Based TMR Circuits" to learn more about clock domains.
* Clean up/add to Project X-Ray, bit2fasm, and FASM modules on the Computing Boot Camp website.

#### Daily Updates

* **Monday**:
  * Memorial Day
* **Tuesday**: 
  * Meeting about SpyDrNet-SHREC.
  * Started going through SpyDrNet-SHREC API
* **Wednesday**: 
  * Worked on FASM page for the Computing Boot Camp and added more resources for it.
  * Continued going through SpyDrNet-SHREC API
* **Thursday**: 
  * Updated Project X-Ray page on Computing Boot Camp
  * Fixed Project X-Ray documentation for quickstart guide and submitted pull request.
  * Refreshed my memory on the Bit-Inspector code base by going through it with different examples to get ready to meet with Cody and Jacob.
  * Met with Cody and Jacob to talk about bit inspector and how it can be useful for them.
* **Friday**:
  * Studied all the algorithms from TMR paper.
### Week 5: 24 MAY 2021

#### Goals

* Create list of enhancements/features for new SpyDrNet SHREC release
  * Documentation
  * Examples
  * New features?
  * Bugs?
* Review SpyDrNet SHREC testing infrastructure
* Create some TMR examples that can be downloaded to board
* Continue reading "Synchronization Voter Insertion Algorithms for FPGA Designs Using Triple Modular Redundancy" paper to understand best algorithm that is also used in SpyDrNet SHREC
* Continue working on main page for SpyDrNet-SHREC
* Start working on basic tutorial for SpyDrNet-SHREC

#### Daily Updates

* **Monday**:
  * Explored creating netlists that can be downloaded to a board.
* **Tuesday**: 
  * Created a simple two-bit counter with one-shot detection, and successfully applied TMR to the netlist, and downloaded it to a board. I only triplicated the LED port, and manually changed the constraints so the all three copies of the counter output (2 x 3 = 6 LEDs for the output), so that all three of the replicates can be viewed. 
* **Wednesday**: 
  * Attended Deep dive meeting.
  * Attended short bootcamp meeting.
  * Finished creating two-bit counter with documentation.
  * Added to two-bit counter example to allow for generating a bitstream from the python script. This took some time to figure out how to generate a bitstream from a netlist. Currently it is just an option in the script (a boolean flag), but I thought it would be worthwhile and convenient to have to script create the bitstream from the netlist automatically. Might be useful for future examples as well.
* **Thursday**: 
  * Tried to run pytest for SpyDrNet SHREC. It is having trouble finding the 'spydrnet' package, and so the tests fail.
  * Read TMR paper and learned about the four different voter types: reducing, partitioning, clock domain crossing, and synchronization. 
  * Learned about illegal voter locations in an FPGA, how voters are inserted, and the some of the algorithms behind finding where to place voters. 
* **Friday**:
  * Met with Andrew to talk about new features for SpyDrNet SHREC.
  * Continued reading TMR paper. 

### Week 4: 17 MAY 2021

#### Goals

* Finish SpyDrNet Vivado examples
* Finish reading "Synchronization Voter Insertion Algorithms for FPGA Designs Using Triple Modular Redundancy" paper
* Create "Install" page and main page for SpyDrNet-SHREC
* Create three simple TMR examples
* Put "How To Contribute" page on Computing Bootcamp website, and start fixing other units to fit the format

#### Daily Updates

* **Monday**:
  * Created another Vivado example in which it is explained how to create/view a netlist inside Vivado. 
  * Attended SpyDrNet meeting. I'll continue working on the Vivado examples for SpyDrNet, and work on creating some simple examples for SpyDrNet SHREC.
* **Tuesday**: 
  * Finished all 3 Vivado examples and created a branch for them.
* **Wednesday**: 
  * Created IMMERSE Summer 2021 proposal. 
  * Attended DEEP DIVE presentation on diversity.
  * Attended Computing Boot Camp meeting
  * Continued reading TMR paper
* **Thursday**: 
  * Worked on creating new SpyDrNet SHREC examples. Got lost in the SHREC API, but hopefully meeting with Andrew will help with that. 
  * Worked on main page for SpyDrNet SHREC. We don't know a lot about the functionality of the tool, so we need
  * Created pull request for "How to Contribue" page for Computing Boot Camp
* **Friday**:
  * Looked at plot_generic_tmr.py script from SpyDrNet SHREC in more depth to see what was going on, and came up with a list of questions for Andrew.
  * Met with Andrew and had a great discussion on SpyDrNet SHREC to learn more about it and its purpose. We have more things to add to the documentation now, and we also understand a lot more about it now.
  * Prepared for SpyDrNet 1.8.1 release by going over the release notes on the wiki

### Week 3: 10 MAY 2021

* **Monday**:
  * Finished LUT_builder python script and tested it with my BASYS3 board. It seems to work just fine, only requiring a constraints file to be created. Added comments and changed code for better readability. 
  * Attended hirel-tools meeting. 
  * Attended bootcamp meeting for Python.
* **Tuesday**: 
  * Created Bootcamp "How to Contribute" page.
* **Wednesday**: 
  * Created some simple SystemVerilog files for the SpyDrNet Vivado example
* **Thursday**: 
  * Learned a little bit on how to use Sphinx so I can rebuild the SpyDrNet docs and insert the Vivado examples. I came up with three different examples that would be helpful: Getting EDIF from a design in Vivado and parsing it into SpyDrNet, creating EDIF from scratch with SpyDrNet and downloading it to an FPGA board, and modify a pre-existing netlist by parsing it with SpyDrNet and then composing the file after modifications have been made.
  * Started adding some .rst documentation for the EDIF from scratch example.
* **Friday**:
  * Jacob and I collaberated on what we had both learned from SpyDrNet and tried to figure out more about what we should change for the documentation.
  * We also went over all the TMR documentation and created issues in GitHub for everything we could add/change to the documentation.
  * Had a meeting with SpyDrNet team to discuss the upcoming 1.8.1 release, as well as what we plan on doing for the 1.9.0 release in the future (some reorganization of the docs, and some new shortcuts and features)

### Week 2: 3 MAY 2021

* **Monday**:
  * Went to tools meeting. I need to do more tutorials on SpyDrNet. I haven't done anything with netlist manipulation yet, only parsing and composing. I'll continue to try and get TMR to work with some of my own designs and then upload them to my baord.
  * Used TMR to triplicate some simple designs. Tried different settings i.e. triplicating/not triplicating top-level ports, adding voters. Spent time trying to understand the tool and how it works.
  * Started to get my RISCV processor netlist ready for TMR, but had some trouble with synthesis on lab machine. Maybe my Vivado is too old of a version? Either way, I was able to get the netlist from a different machine. TMR did not work on my RISCV processor though, I got a warning saying "feedback cannot be broken," and the error ultimately occurs saying: "AttributeError: 'NoneType' object has no attribute 'add_cable'"
* **Tuesday**: 
  * Finished Bit-Inspector presentation for tomorrow. Added graphics for easier understanding.
  * Started reading though "Synchronization Voter Insertion Algorithms for FPGA Designs Using Triple Modular Redundancy" paper. I've learned a lot about TMR and understand more about voters and their implementation.
  * Tried getting Remote Desktop Protocol working in case I ever need to use it for working remotely. Couldn't quite figure it out unfortunately, but I can still SSH into the machine. I wanted to get RDP working for using Vivado or other GUI based things.
* **Wednesday**: 
  * Refined and practiced Bit-Inspector presentation and made sure I could use the projector for the presentation.
  * Went to IMMERSE meeting on ethics. Interesting conversation on duty vs charity driven service
  * Went to track meeting and presented on the Bit-Inspector
  * Discussed plans for Computing Boot Camp and individual responsibilites in meeting.
  * Started creating a netlist from scratch with SpyDrNet that I can generate a bitstream from
* **Thursday**: 
  * Worked on creating a new SpyDrNet example in which a netlist is created that can be downloaded onto a Nexys4 board. It is similar to the existing 'minimal.py' example, but instead implements a LUT using primitives compatible with the FPGA. So far it has helped me a lot to get hands on experience with the tool. I've been working with a netlist generated from Vivado, and working from there. The plan is to get a netlist that I could put into a Post-Synthesis project and generate a bitstream from it.
* **Friday**:
  * Continued working on SpyDrNet netlist from scratch example. I've made some changes to make it parameterizable, perhaps adding the ability to use different sizes of LUTs.

### Week 1: 26 APRIL 2021

* **Monday**:
  * Set up office space.
  * Met with Dallin and Jordi to start with SpyDrNet.
  * Attended BootCamp meeting.
* **Tuesday**: 
  * Installed Ubuntu on new office machine and set up environment.
  * Made this website. :)
  * Setup SSH for remote work.
  * Added my website link to Computing Boot Camp website.
  * Learned a lot about Python virtual environments, very helpful for not breaking stuff. 
  * Started trying to understand pytest. Will probably spend more time on this another day.
  * Got Vivado up and running on my machine.
  * Created a small design with an AND gate module instanced two times inside a top module.
  * Generated edif file in the TCL console with `write_edif my_netlist.edif` and opened it up in SpyDrNet to try and make sense of it.
* **Wednesday**: 
  * Reinstalled Project X-Ray and got it running correctly. Found an issue with a "resources.yaml" file that should be generated automatically, but for some reason did not generate for me, so I will create an issue on the Project X-Ray page.
  * Got Bit Inspector working again with the simple andgate design I made earlier. I could probably simplify the code that is contained in Bit Inspector before handing it off, could make the design easier to read.
  * Changed presentation from last year to reflect progress with the Bit Inspector tool. Since the Bit Inspector tool hadn't been finished yet when I gave the presentation, I basically changed most of the presentation to talk about that instead of the modified bit2fasm tool I was working on. The presentation is mostly ready, but still needs some work.
* **Thursday**: 
  * Started working Python tutorials from here: https://docs.python.org/3/tutorial/. Did Section 1-4.6, and feel more confident now. I plan on working through the rest of the tutorials later
  * Read and understood "/examples/basic/plot_stat.py" to better understand netlist hierarchy and how to print it. I am keeping a running list of questions about SpyDrNet that I can ask Dallin and Jordi
  * Started working to understand "/examples/basic/plot_single_use_definitions.py" I think I understand the idea behind it, but I haven't been able to see what the script outputs.
* **Friday**: 
  * Spoke with Dallin and he answered all of my questions. I feel pretty confident with the basic workings of SpyDrNet, but I haven't dived deep into all of the different functions and examples.
  * Started reading through the SpyDrNet-SRHEC documentation. I am keeping my own list of notes to try and understand the documentation, as well as ideas for better documentation.
  

  
<!-- 
Log Template

### Week N: 2021

#### Goals

#### Daily Updates

* **Monday**:
  * 
* **Tuesday**: 
  * 
* **Wednesday**: 
  * 
* **Thursday**: 
  * 
* **Friday**:
  *
 -->
