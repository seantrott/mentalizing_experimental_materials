# Experimental materials for investigating mentalizing and pragmatic inference

This repository contains the JsPsych code to run the online experiments described in Trott and Bergen (*Discourse Processes*, to appear). 

## Dependencies

The code assumes that *JsPsych* (found [here](https://www.jspsych.org/)) has been downloaded and is located in the same directory as the experimental code.

Additionally, this code was written with **version 5.0.03** of JsPsych in mind (there may be incompatibilities with the newest version).

Finally, there are a couple of path/file-dependent functions:

### **Saving the data**

Attached is a .php script (*save_data.php*) which can be used to save the data from the experiment onto a server. Replace *{INTENDED_FILEPATH}* with the path you want to use:

```
$filename = "my_server/data".$_POST['filename'];
```

### **Consent page**

There is also an .html page, *consent.html*, which embeds a consent form in the web browser (and is then referenced by the main experiment script), allowing participants to explicitly mark their consent to the experiment. Replace *{CONSENT_FILE.pdf}* with the path to the appropriate consent file, e.g.

```
<embed src="lab_consent_file.pdf" width="800px" height="1100px" />
```

## Relevant variables

Participants are randomly assigned to one of two lists (*group1* or *group2*), coded in the **condition** variable.

Participants are also randomly assigned a **subject_id** (variable name), and a **survey_code** (variable name). 

The critical stimuli in the indirect requests task are coded according to their **stimulus type** as *belief* or *no_belief* (corresponding to Speaker Aware and Speaker Unaware from the paper, respectively).

Answers to the Short Story Task (SST) are coded as *sst* (for the **stimType** variable). 

Answers to the preliminary SST questions are coded as *sst_general* (for the **stimType** variable).

The number of a given item is coded as **stimNum**.

Information about a participant's gender and whether they are a native English speaker is coded as *demographic1* in the **stimType** variable. 

Finally, information about a participant's age and what they thought the experiment was about is coded as *demographic2* in the **stimType** variable.

## Differences between experiments

The only difference between Experiment 2 and Experiment 3, as described in Trott and Bergen (2018), is the target question: in Experiment 2, participants are asked to make a paragraph judgment, and in Experiment 3, they explicitly indicate whether they thought the speaker was making a request.

## Contact

For questions, please contact Sean Trott at sttrott (at) ucsd dot edu.