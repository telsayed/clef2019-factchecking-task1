This folder contains 7 files.
<br>
Their format is identical to that in the training set, except that the fourth column is missing.  
For instance, 20151219_3_dem.tsv looks like this:

> 1	RADDATZ	Good evening to you all. <br>
> 2	RADDATZ	The rules for tonight are very basic and have been agreed to by all three campaigns in advance. <br>
> 3	RADDATZ	Candidates can take up to a minute-and-a-half to respond directly to a question. <br>
> 4	RADDATZ	For a rebuttal, for a follow-up, 45 seconds will be allowed. <br>
> [...]

The folder [data](../) contains also a submission_instance_en.zip file that is an example of what we 
expect the participants to submit: <br>

* One readme file:						README.txt <br>
* Seven primary prediction files: 		primary___filename__.txt <br>
* Seven contrastive 1 prediction files:	contrastive1___filename__.txt <br>
* Seven contrastive 2 prediction files:	contrastive2___filename__.txt <br>

Where __filename__ is in [20151219_3_dem, 20160129_7_gop, 20160311_12_gop, 20180131_state_union, 20181015_60_min, 20190205_trump_state, 20190215_trump_emergency]

That is, this hypothetical participant has submitted the results of one primary and two contrastive runs. <br>

The readme and the seven primary files are mandatory. The contrastive files are optional.  <br>

Note that whereas the participants are free to name the ZIP file(s) at will, the readme, the primary, and the  <br>
contrastive files must stick to the above naming conventions. Failing to stick to them will cause the <br>
submission to be rejected.<br>

The README.txt must contain the following:<br>

````
1. Team ID 
2. Team affiliation 
3. Contact information 
4. System specs
- 4.1 Core approach 
- 4.3 Important/interesting/novel novel representations used (features, embeddings...)
- 4.4 Important/interesting/novel tools used
- 4.5 Significant data pre/post-processing
- 4.6 Other data used (outside of the provided)
5 References (if applicable)
````

The example ZIP file contains both a template and an example. <br>

The primary and the contrastive files should have the same format as those used during training: tab-separated id and 
judgment; one instance per line. From the example 20151219_3_dem.tsv:

> [...] <br>
> 18	0.880493290088 <br>
> 19	0.992619629045 <br>
> 20	0.346526163744 <br>
> [...]

We have implemented some checkers, but it is still the responsibility of the participants to double-check that 
their submissions are correct. <br>

As a reminder, participants can submit predictions more than once, but only the last one before the deadline 
(6 May 2019) will be evaluated and considered as official. 
