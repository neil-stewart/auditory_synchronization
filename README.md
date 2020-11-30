# Data and code for Reimers and Stewart (2016)

Reimers, S., & Stewart, N. (2016). Auditory presentation and synchronization in Adobe Flash and HTML5/JavaScript web experiments. Behaviour Research Methods, 48, 897-908. [doi: 10.3758/s13428-016-0758-5](http://dx.doi.org/10.3758/s13428-016-0758-5)

As on the journal website.

This repo file contains the following:

## Code

Code used for running the experiment and analysing the data. Comprises:

* Flash_code: Contains the flash code used to run the tests, both non-compiled .fla and compiled .swf code (Study 1 = sep; Study 2 = sync)

* JavaScript_code: Contains the HTML-CSS3-JavaScript code used to run the tests (Study 1 = sep; Study 2 = sync; Study 3 = jswa; Study 4 = jswa2)

* R_Code: R code for taking the data in the the csv files and plotting the graphs

## Data

CSV files for all the data reported in the paper.

* The filenames are of the format condition-machine-browser-implementation[-repetition][-wav].csv

* condition: sep [separate calls for auditory and visual presentation as in Study 1]

* machine: officepc [windows 7 desktop]; lenlap [lower spec Lenovo Laptop]

* browser: ie [Microsoft Internet Explorer]; ed [Microsoft Edge]; ff [Firefox]; cr [Chrome]

* implementation: js [JavaScript]; fl [Flash]

* repetition: not included for first run

* wav: All tests used mp3 audio file, unless -wav was in the filename, meaning it used a wav file

## Logs

A dump of logs from the Black Box Toolkit, for the runs. There are more files here than in the csv dataset because:

(a) We did some extra tests (e.g., using wav rather than mp3 audio for the stuff in Studies 1 and 2), which didn't improve synchronization, so were dropped

(b) We had to repeat some of the tests because of, for example, extraneous noises triggering the audio input

* I renamed the data files for clarity, so they don't completely match the BBTK logs in filename

* However, the date stamps should make it easy to match them up - at the end of a run I pasted the results from BBTK into a csv file and saved both

* These should be redundant, as the output data are the same as in the csv files. But they're included for completeness.


