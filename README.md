# Experimental materials for investigating mentalizing and pragmatic inference

This repository contains the JsPsych code to run the online experiments described in Trott and Bergen (Discourse Processes, to appear). 

## Dependencies

The code assumes that *JsPsych* (found [here](https://www.jspsych.org/)) has been downloaded and is located in the same directory as the experimental code.

Additionally, this code was written with **version 5.0.03** of JsPsych in mind (there may be incompatibilities with the newest version).

Finally, there are a couple of path/file-dependent functions:

* **Saving the data**: Attached is a .php script (*save_data.php*) which can be used to save the data from the experiment onto a server. Replace *{INTENDED_FILEPATH}* with the path you want to use.  
* **Consent page**: There is also an .html page, *consent.html*, which embeds a consent form in the web browser (and is then referenced by the main experiment script), allowing participants to explicitly mark their consent to the experiment. Replace *{CONSENT_FILE.pdf}* with the path to the appropriate consent file.
