# Eye Gaze Metrics Extraction


This folder contains 5 Python scripts that analyze eye gaze metrics, patch characteristics, and survey data from the experiment. Below is a detailed description of each script and the required files to run them:

1. fixation_generator.ipynb
This script processes raw eye metrics data from participants to generate various eye gaze metrics, including fixation count, fixation rate, total fixation time, average fixation duration, and the first fixation on the main six Areas of Interest (AOIs) in the experiment. It also includes patch correctness and participants' acceptance/rejection decisions.

Requirements:
•	raw_data/: Contains CSV files for each participant per task, including raw eye gaze metrics and participant information such as ID, patch order, and acceptance/rejection.
•	java-info.xlsx: Includes the lines of code for methods and classes in the source code file and test file for each patch, along with patch correctness data.

Output:
•	generated_fixations/: Contains the fixation metrics, patch correctness, and participants' acceptance/rejection data, both separately and merged into a single Excel file.

2. fixation_survey_generator.ipynb
This script generates all the fixation metrics, similar to fixation_generator.ipynb, but also includes survey results from the participants.

Requirements:
•	raw_data/
•	java-info.xlsx
•	surveys/: Contains Excel files with participants' survey responses.

Output:
•	generated_fixations_surveys/: Contains fixation metrics along with survey results.

3. bug_report_AOIs_generator.ipynb
This script generates fixation counts, fixation times, and average fixation durations for each participant, specifically targeting the defined AOIs in the bug report file.

Requirements:
•	raw_data/
•	java-info.xlsx
•	bug-info.xlsx: Includes the lines of code for different AOIs in the bug report file.

Output:
•	generated_bug_report_AOIs/: Contains the generated AOI-specific fixation data.

4. time_calculator.ipynb
This script calculates the total time (in milliseconds) that each participant spent on each task.

Requirements:
•	raw_data_times/: Contains XML files for each participant per task.

Output:
•	calculated_time/: Contains the calculated time spent by participants on each task.

5. eye_gaze_coordination_generator.ipynb
This script visualizes the fixations of a single participant on a single task using eye gaze coordination data.

Requirements:
•	raw_data_times/
•	bug1-1.png: A screenshot of the IDE where participants were working on the task.

Output:
•	generated_eye_gaze_coordination/: Contains the visualizations of the fixation eye gaze coordination. Note: The accuracy of these visualizations may be limited due to participants scrolling within the IDE during the experiment.
 
This README provides an overview of each script, including the necessary files and expected output, making it easier for users to understand and run the analyses.

