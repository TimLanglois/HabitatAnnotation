# R workflow 
Example workflow using R to format and calculate point scores, mean and sd rugosity and % habitat cover from Habitat annotation applied using the TransectMeasure software from www.seagis.com.au.

This annotation schema and R script is described and included in a published paper<sup>1</sup>, please cite if you use it.
Please refer to this GitHub repository for updated versions of the annotation schema and R script.

<HR>
</HR>

<b>Table of contents</b>

[Example R script](#method)<br></br>
[Example data](#transectmeasure-example)<br></br>
[Example output data and plot](#output-example)<br></br>
[Folder structure](#introduction)<br></br>
[Bibliography](#bibliography)

<HR>
</HR>

#<a name="method"></a>Example R script

The example <a href="https://github.com/TimLanglois/HabitatAnnotation/blob/master/x_ExampleR_0_HabitatAnnotation_Format.and.write.data_170519.R">R script</a> is designed to import and format the raw annotation output from TransectMeasure and calculate point scores, mean and sd rugosity and % habitat cover.

The script uses Data Wrangling grammar from the tidyr<sup>2</sup> and dplyr<sup>3</sup> packages and data piplines. These packages should be cited if you use the script.
For more information on the grammar of tidyr and dplyr see the <a href="https://www.rstudio.com/wp-content/uploads/2015/02/data-wrangling-cheatsheet.pdf">Data Wrangling cheat sheet</a>. 

<HR>
</HR>

#<a name="transectmeasure-example"></a>Example annotation data

An example of <a href="https://github.com/TimLanglois/HabitatAnnotation/blob/master/x_ExampleData_BRUV_TM_HabitatAnnotation.txt">habitat annotation data</a> generated from the TransectMeasure software is provided that will run with the above script.

<HR>
</HR>

#<a name="output-example"></a>Example output data and plot

The script will produve two outputs:

The first is a summary of the habitat and relief annotation as <a href="https://github.com/TimLanglois/HabitatAnnotation/blob/master/x_ExampleOutput_habitat.point.score.csv" >point scores </a>, this output will be easily comparable to any outputs produced by squidle+ and will be useful for modeling habitat occurence.

The second is a summary of the habitat and relief annotation as <a href="https://github.com/TimLanglois/HabitatAnnotation/blob/master/x_ExampleOutput_habitat.percent.cover.and.mean.and.sd.of.relief.csv">percent cover and mean and SD of relief </a>, this output is more directly useful in data analysis of fish/habitat associations and is directly comparable to other visual estimates of habitat cover.

A simple plot of the habitat data expected from the R script is provided below.

![alt text](https://cloud.githubusercontent.com/assets/14978794/26228361/b6e06392-3c6b-11e7-8c33-013507b0c8f8.png "Example plot of habitat data")






<HR>
</HR>

#<a name="introduction"></a>Folder structure

The above script assumes that you have a folder strucutre following this format:

![alt text](https://cloud.githubusercontent.com/assets/14978794/18631738/5438d4a0-7ea6-11e6-83b4-9795445876b9.png "Example folder structure")


<HR>
</HR>

#<a name="bibliography"></a>Bibliography

1. McLean, Dianne L., Tim J. Langlois, Stephen J. Newman, Thomas H. Holmes, Matthew J. Birt, Katrina R. Bornt, Todd Bond, et al. 2016. “Distribution, Abundance, Diversity and Habitat Associations of Fishes across a Bioregion Experiencing Rapid Coastal Development.” Estuarine, Coastal and Shelf Science 178 (September): 36–47.
<br></br>
2. Hadley Wickham (2016). tidyr: Easily Tidy Data with `spread()` and `gather()` Functions. R package version 0.4.1.
  https://CRAN.R-project.org/package=tidyr
<br></br>
3. Hadley Wickham and Romain Francois (2015). dplyr: A Grammar of Data Manipulation. R package version 0.4.3.
  https://CRAN.R-project.org/package=dplyr

