YouTube Transcript Notes Generator

This Python script fetches the transcript of a YouTube video using its video ID and saves it in a "notes" format in a text file. It is particularly useful for creating time-stamped notes for educational or content-review purposes.

Features
- Fetches transcripts directly from YouTube.
- Formats the transcript with timestamps in `[MM:SS]` format.
- Saves the transcript into a readable text file.



Prerequisites
Install Required Libraries
1. Ensure you have Python installed on your system (version 3.7 or later).
2. Install the `youtube-transcript-api` library by running the following command:
   bash
   pip install youtube-transcript-api
   



How to Use

1. Clone or Download the Script
Save the script file in a directory of your choice. Name it, for example, `save_transcript.py`.

2. Replace the YouTube Video ID
Locate the line in the script where `video_id` is defined:
python
video_id = "dQw4w9WgXcQ"  Example video ID

Replace `dQw4w9WgXcQ` with the actual YouTube video ID. The video ID is the part of the URL after `v=`. For example:
- URL: `https://www.youtube.com/watch?v=abcd1234`
- Video ID: `abcd1234`

3. Run the Script
Run the script using the command line or an IDE:
bash
python save_transcript.py


4. Output File
The script will generate a text file named `transcript_notes.txt` in the same directory. This file will contain the transcript in the following format:

[00:05] This is the first line of the transcript.
[00:12] Here is the second line of the transcript.
[00:25] And the third line of the transcript appears here.




Customization
Change the Output File Name
You can modify the output file name by updating the `output_filename` variable:
python
output_filename = "my_notes.txt"




Error Handling
Common Issues
1. Transcript Not Available:
   If the transcript is not available for a video (e.g., the video owner has disabled it), an error will be displayed.
   
   An error occurred: No transcripts were found for the given video ID.
   

2. Network Issues:
   Ensure your internet connection is stable when running the script.

Debugging Tips
If you encounter any errors, verify the following:
- The video ID is correct.
- The transcript is enabled for the video.



License
This script is free to use and distribute under the MIT License.



Contributions
Feel free to contribute to this project by submitting pull requests or reporting issues. Your feedback is appreciated!
