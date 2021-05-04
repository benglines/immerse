---
layout: default
title: IMMERSE Log
---

## Schedule

* **Monday**:
  * 7:00am-12:00pm, 1:00pm-6:00pm
* **Tuesday**: 
  * 7:00am-12:00pm, 1:00pm-6:00pm
* **Wednesday**: 
  * 7:00am-12:00pm, 1:00pm-6:00pm
* **Thursday**: 
  * 7:00am-12:00pm, 1:00pm-6:00pm

## Log

### Week 2: 2 MAY 2021

* **Monday**:
  * Went to tools meeting. I need to do more tutorials on SpyDrNet. I haven't done anything with netlist manipulation yet, only parsing and composing. I'll continue to try and get TMR to work with some of my own designs and then upload them to my baord.
  * Used TMR to triplicate some simple designs. Tried different settings i.e. triplicating/not triplicating top-level ports, adding voters. Spent time trying to understand the tool and how it works.
  * Started to get my RISCV processor netlist ready for TMR, but had some trouble with synthesis on lab machine. Maybe my Vivado is too old of a version? Either way, I was able to get the netlist from a different machine. TMR did not work on my RISCV processor though, I got a warning saying "feedback cannot be broken," and the error ultimately occurs saying: "AttributeError: 'NoneType' object has no attribute 'add_cable'"
* **Tuesday**: 
  * 
* **Wednesday**: 
  * 
* **Thursday**: 
  * 
* **Friday**:

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

* **Monday**:
  * 
* **Tuesday**: 
  * 
* **Wednesday**: 
  * 
* **Thursday**: 
  * 
* **Friday**:
 -->
