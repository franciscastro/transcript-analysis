# transcript-analysis
Code library for transcript analysis for research projects

## `transcript-process-docs-to-sheets.ipynb`
This `.ipynb` is used to process Zoom-produced transcripts stored as Google Doc files into a Google Sheets file. 

The transcript data compiled into the resulting Sheets file is organized under the following columns: 
1. Line Number
2. Start time (of the utterance)
3. End time (of the utterance)
4. Speaker
5. Utterance

### Use of Gemini
This `.ipynb` was generated with the assistance of Google Gemini and was modified by the author to customize according to the needs of the research project. 

The prompts are added here for documentation purposes. 

#### Prompt 1
> I need a program that will organize content from a google doc into a google sheet. The doc contains transcripts from an interview. 
> 
> An utterance in the doc is identified by a line number, the timestamp of the utterance, and the text that corresponds to the utterance made by the speaker. Each of these are in their own lines in the doc. When organized in the sheets, these need to be in their own columns. Additionally, the last line that has the utterance has both the name of the speaker and the actual statement made by the speaker, separated by a colon. These need to be separated into their own respective columns in the sheet as well. 
> 
> A sample input from a doc is below: 
> 
> 1 <br />
> 00:00:00.070 --> 00:00:01.070 <br />
> John Doe: Sounds good. 
> 
> 2 <br />
> 00:00:02.530 --> 00:00:07.360 <br />
> Jane Doe: Oh, thank goodness that time it worked. Okay, so… Now.
