# HabitatAnnotation
Habitat annotation of horizontally facing benthic imagery from baited and unbaited remote stereo-video deployments and diver swum stereo-video transects. With an applied example using the TransectMeasure software from www.seagis.com.au

<HR>
</HR>

<b>Table of contents</b>

[Introduction](#introduction)<br></br>
[Method](#method)<br></br>
[Recommended approaches](#recommended-approaches)<br></br>
[TransectMeasure example](#transectmeasure-example)<br></br>
[Bibliography](#bibliography)

#<a name="introduction"></a>Introduction

We have developed a simple approach to characterise the composition and complexity of habitats from horizontally facing benthic imagery, adapting existing standardised schema for benthic composition (<a href="https://github.com/TimLanglois/HabitatAnnotation/blob/master/CATAMI-visual-guide-latest.pdf">CATAMI classification scheme</a><sup>1</sup>) and benthic complexity<sup>2</sup>, with the addition of a class to quantify the % of benthos versus open water within the horizontally facing image. 

The annotation approach is rapid and produces % composition and mean and standard deviation estimates of complexity which enable flexible modeling of habitat occurrence and habitat-fish relationships.

This annotation schema is described and included in a published paper<sup>3</sup>, please cite if you use it.
Please refer to this GitHub repository for updated versions of the annotation schema.

Parts of this annotation scheme have also been trailed in two further published papers<sup>4,5</sup>.

<HR>
</HR>

To simplify the annotation process and still represent multiple scales of habitat in horizontaly facing imagery, we have gridded the images in 5 x 4 cells.

Protocol: each of the cells is annotated for dominant Benthic Composition, Field of View and Relief.

![alt text](https://cloud.githubusercontent.com/assets/14978794/17895290/3628ea54-697f-11e6-80c0-3633435d75f9.PNG "Application of annotation approach to characterise benthic composition and benthic complexity from horizontally facing remote video or from diver swum transects. Using TransectMeasure software")

<HR>
</HR>

#<a name="method"></a>Method

The annotation schema is made up of nested Benthic Composition classes taken from the CATAMI schema and a Field of View and Relief class that are useful for characterising horizonatlly facing imagery.
BROAD>MORPHOLOGY>TYPE/FieldOfView/Relief

For detailed information on the particular taxanomic levels within the BROAD>MORPHOLOGY>TYPE classifications provided in this annotation schema, please consult the CATAMI visual guide within this repository.


To the BROAD class, we have added additional levels of "Open Water", to calculate the % of benthos within each image, and "Unknown", to account for the frequent issues of limited visibility typical for forward facing imagery.


The FieldOfView class allows the qualification of the image quality within each cell and the "Limited" level is used where benthos or substrate obscurs the cell within ~1m of the camera (typically the length of the diode arm of baited stereo-video systems)

Definition of FoV options:
o	Facing Down: No open water visible.
o	Facing Up: No substrate visible.
o	Limited: BRUV visibly landed on its side or the FoV is obstructed by benthos or substrate within 1m of camera (length of diode arm).
o	Open: BRUV landed upright and level on the substrate and there is an adequate amount of habitat available for classification.


The Relief class uses a 0-5 quatification of relief <sup>2</sup> and includes and "Unknown" level to account for cells with limited visibility.
When the “BROAD” is “Open Water”, “Relief” should be classified as “Unknown”.
o	 “Relief” type is representative of complexity or the height and angle of substrate. 
o	 Distinct categories have been adapted from Wilson et al. (2006):
0.	Flat substrate, sandy, rubble with few features. ~0 substrate slope.
1.	Some relief features amongst mostly flat substrate/sand/rubble. <45 degree substrate slope.
2.	Mostly relief features amongst some flat substrate or rubble. ~45 substrate slope.
3.	Good relief structure with some overhangs. >45 substrate slope.
4.	High structural complexity, fissures and caves. Vertical wall. ~90 substrate slope.
5.	Exceptional structural complexity, numerous large holes and caves. Vertical wall. ~90 substrate slope.

<HR>
</HR>

#<a name="recommended-approaches"></a>Recommended approaches

<b>Standard (rapid) assessment</b> of Benthic Composition, Field of View and Relief we recommend using ONLY the:
BROAD/FieldOfView/Relief classes. 
An experienced analyst would be able to annotate this schema to over 200 images a day.
<br></br>
OR
<br></br>
<b>Detailed assessment</b> of Benthic Composition (where coral bleaching or macroalgae compostion was of interest), Field of View and Relief we recommend using all the classes in the schema:
BROAD>MORPHOLOGY>TYPE/FieldOfView/Relief classes. 
An experienced analyst would be able to annotate this schema to over 120 images a day.

<HR>
</HR>

#<a name="transectmeasure-example"></a>TransectMeasure example

The annotation schema has been applied using the TransectMeasure software from www.seagis.com.au and the  <a href="https://github.com/TimLanglois/HabitatAnnotation/blob/master/Transect%20Measure%20Habitat%20Codes_160705.txt">configuration text file</a> for uploading the schema to TransectMeasure is provided in this repository.

We also provide a <a href="https://github.com/TimLanglois/HabitatAnnotation/blob/master/2_Standard%20Operating%20Procedure_TransectMeasure.md">TransectMeasure Standard Operating Procedure</a>. 

<HR>
</HR>

#<a name="bibliography"></a>Bibliography

1. Hill, N., Althaus, F., Rees, T., et al., 2014. CATAMI Classification Scheme for Scoring Marine Biota and Substrata in Underwater Imagery Version 1.4: December 2014
<br></br>
2. Wilson, S. K., N. A. J. Graham, and N. V. C. Polunin. 2006. “Appraisal of Visual Assessments of Habitat Complexity and Benthic Composition on Coral Reefs.” Marine Biology 151 (3). Springer-Verlag: 1069–76.
<br></br>
3. McLean, Dianne L., Tim J. Langlois, Stephen J. Newman, Thomas H. Holmes, Matthew J. Birt, Katrina R. Bornt, Todd Bond, et al. 2016. “Distribution, Abundance, Diversity and Habitat Associations of Fishes across a Bioregion Experiencing Rapid Coastal Development.” Estuarine, Coastal and Shelf Science 178 (September): 36–47.
<br></br>
4. Collins, Danielle, Tim J. Langlois, Todd Bond, Thomas H. Holmes, Euan S. Harvey, Rebecca Fisher Dianne L. McLean. In press. “A novel stereo-video method to investigate fish-habitat relationships.” Methods in Ecology and Evolution.
<br></br>
5. Katherine Bennett, Tim Langlois , George Shedrawi , Shaun Wilson, Dianne McLean. In press. “Can Diver Operated Stereo-Video Surveys for Fish Be Used to Collect Meaningful Data on Benthic Coral Reef Communities?” Limnology and Oceanography, Methods / ASLO.