# NRC-readalong
NRC read along project

Indigenous Languages Technology Project 
Digital Technologies Research Centre 
National Research Council Canada 

## Background
The Indigenous Languages Technology Project includes a project on the creation of “read alongs” for teaching 
Indigenous languages – i.e. interactive text-audio documents where words are highlighted as they are spoken. 
Language activists and teachers in communities often have collections of written text that have been read by 
fluent speakers of the language, which are intended to help teach language learners. However, when a learner 
is just beginning, it can be difficult to follow along and figure out which word is being read out. ReadAlong 
Studio helps the learner by aligning the text and audio streams together, so that the language learner can see 
the individual words highlighted as they are being spoken in the audio. 
Creating such readalongs, even with the Studio, can be challenging. There can be issues with the grapheme-
to-phoneme (g2p) conversion of the text, a step required to perform alignment, or with the quality of the 
recording, or with the alignment of long text/audio pairs, to name just a few. 
Recently, the NRC team has added a prototype web app to make it easier for users to create read-alongs 
without the need to install the Python software themselves or the need to learn to work with a Command Line 
Interface (CLI), something most language teachers are not familiar with. 

## Your Challenge
The read-alongs web app is built on the ReadAlong Web Component, with the editable mode enabled. Your 
challenge will be to improve the editable ReadAlong Web Component to include editable header and 
subheader (§1), to support image insertion for each page (§2), and to facilitate adding translations (§3).  
The Web Component is written using Stencil JS. It is initialized with a structured text file (XML) produced by 
ReadAlong Studio, an audio file, and an alignment file (SMIL). The web component is designed to run both 
online and offline. In offline mode, each asset (audio, text, alignment) file is Base64 encoded and embedded 
within a single HTML file. 
The Web Component is used in the ReadAlong Studio Web Application (written in Angular) for both editing and 
presentation purposes. After a user aligns their text and audio, they should be presented with an editable web 
component rendering their ReadAlong. The following should be editable only when the Web Component is 
initialized in ‘editable’ mode: 

### Milestone 1: Title, Headers and Subheaders 
Each ReadAlong should have the web page title (shown in the browser tab), header (shown above the read-
along) and subheader/subtitle (shown right under the header) editable. The edits here should persist in any 
future instances of the Web Component. See Figure 1 for an example. 
 
ReadAlong Studio Software Engineering Project Proposal 
### Milestone 2: Images 
Each ReadAlong should allow for up to one image to be inserted per page. The image should be able to be 
uploaded from the user’s computer, should allow for copyright information, and should be able to be deleted. 
The image should persist in any future instances of the Web Component and should be compressed and 
encoded for inclusion in the single-file HTML offline format. See Figure 1 for an example.  

### Milestone 3: Translations 
Each line in each ReadAlong should allow for a corresponding translation line. These lines should be 
removable and should use the Web Component’s built-in translation classes. See Figure 2 for an example.  
 
Figure 1: Screenshot of Editable Web Component showing editable Header and Subheader (shows as title and 
subtitle in the screenshot) and images 
 
ReadAlong Studio Software Engineering Project Proposal 
 
Figure 2: A read-along with Romanization and translations, each shown as translation lines. 
