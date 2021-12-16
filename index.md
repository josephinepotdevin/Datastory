---
layout: default
---

# <a name="abstr"></a>A few data on women's mis-representation in the media

<div style="text-align: justify"> In <strong>2015</strong>, the Global Media Monitoring Project (GMMP) conducted the largest <a href="https://www.media-diversity.org/additional-files/Who_Makes_the_News_-_Global_Media_Monitoring_Project.pdf">study</a> of women's image, participation and representation in the news media over 20 years and 114 countries. To give an overview on the matter of the significance of women's misrepresentation in the media before 2017, here are some data from this study: </div>
<br>
- Women made up **24%** of the people in newspaper, television, and radio news
- Women made up **20%** of expert featured in TV news
- Women made up **37%** of journalists telling stories around the world
- Women were the subject of political and governmental coverage **16%** of the time
 <div style="text-align: justify"></div>
 <br>
 <div style="text-align: justify">This image of a gendered society reported by the every media can reinforce and perpetuate harmful gender stereotypes. Maybe the MeToo movement had a positive impact on this challenge ?... </div>

# **Table of Contents**
1. [Context](#context)
2. [The Quotebank Dataset](#quotebank)
3. [Descriptive Analysis](#descriptive)
4. [Matched Observational Study](#obsstudy)
5. [First Question of the Study](#first)
6. [Second Question of the Study](#second)
7. [Conclusion of the Analysis](#conclu)


# <a name="context"></a> **Context**: The #MeToo movement 

<div style="text-align: justify"> In 2006, Tarana Burke, activist and sexual assault survivor, creates the MeToo movement in support to all women victims of crimes of sexual nature. It is only in October 2017, when more than 80 women in the film industry made sexual abuse allegations against film producer Harvey Weinstein, that the MeToo movement re-emerged. The actress Alyssa Milano is the one who reignited the movement by encouraging victims of sexual harassment and assault to come forward using the hashtag #MeToo as a status update on Twitter. With the goal of raising awareness of sexual misconduct, empowering survivors to speak out, helping them heal as a community by not feeling alone in this battle, and bringing them justice, the MeToo movement has spread around the world, showing the reality and magnitude of sexual abuse against women.  </div>

<br>

<div style="text-align: justify">The reappearance of this movement can be seen in the newspapers. Indeed, when one analyses the lexical field of thousands of citations from English articles, coming from the <a href="#quotebank">Quotebank Dataset</a>), the rise of #MeToo and the Harvey Weinstein scandal is clearly marked temporally in the two graphs below. The frequency of quoted words related to sexual harassment (sexual harassment, sexual assault, rape, sexual touching) and any references to the #MeToo movement are respectively represented on the left and right figure. Each shows a marked peak of higher frequency in the year 2017 relating the importance that the movement took that year in the newspapers.</div> 

<br>

<img src="D-lex.png" alt="">

<br>

<div style="text-align: justify"> In addition to the movement's instantaneous but temporary effect that can be seen on these graphs, in the long term its beneficial effect is much more profound. Indeed, by inviting thousands of women to come out of the shadows, to protest against such violence, to make themselves heard and to demand justice, these survivors have given the movement an even more important dimension in the fight for gender equality. Indeed, they have empowered the voices of women all around the world.  </div>
<br> 
<div style="text-align: justify"><span style="color:DarkSlateBlue"><strong>It is hoped to find in this analysis, that this empowerment will reverberate through to the newspapers, where women's voices would be better heard, represented, diversified and accepted.</strong></span>  </div>

# <a name="quotebank"></a> **The Quotebank Dataset**: A goldmine of information on the role of women in the media

<div style="text-align: justify"> 178 million quotations along with its speakers extracted from hundreds of english articles from 2015 to 2020 together in one open corpus; that's the <a name="qtdata" href="https://dlab.epfl.ch/people/west/pub/Vaucher-Spitz-Catasta-West_WSDM-21.pdf">QuoteBank Dataset</a>. For a more thorough analysis, additional information about the speakers from the dataset need to be collected. Thus, thanks to an additional speaker metadata available for ~9M speakers (<a href="https://www.wikidata.org/wiki/Wikidata:Main_Page">Wikidata</a>), several attributes were added to the Quotebank dataset to make it more complete: the gender, the date of birth, the academic degree, and finally the speaker's occupations. From here, we have at our disposal a goldmine of information on the subjects, personnalities, genders, careers etcetera represented in the newspaper and displayed to a target audience in the last five years. Nevertheless, the dataset being too important and full of unknown speaker caracteritsics, data processing has been done retrieving only speakers with male or female genders, known ages, academic degrees and occupations for a much more relevant and reliable dataset applicable to <a href="#obsstudy">matched observational studies</a>. A typical line from our edited dataset gives the following informations:</div>
 
 
 <br>
 
<center><span style="color:DarkCyan"><font size="4.5"><i>"At this moment the women of Time's Up and #metoo are looking and saying, why don't we have more stories and why is it that if we see these perversions at the end of the line, why aren't we fixing it at the beginning of the line?"</i></font></span></center>
<br>
<table>
  <tr>
    <td style="background-color: LavenderBlush">Speaker</td>
    <td style="background-color: LavenderBlush">Speaker's Wikidata ID</td>
    <td style="background-color: LavenderBlush">Speaker's gender</td>
    <td style="background-color: LavenderBlush">Speaker's age</td>
  </tr>
  <tr>
    <td>Eric Garcetti</td>
    <td><a href="https://www.wikidata.org/wiki/Q5386557">Q5386557</a></td>
    <td>Male</td>
    <td>47</td>
  </tr>
  <tr>
    <td style="background-color: LavenderBlush">Speaker's occupations</td>
    <td style="background-color: LavenderBlush">Speaker's academic degree</td>
    <td style="background-color: LavenderBlush">Quotation's number of occurences</td>
    <td style="background-color: LavenderBlush">Newspaper's year release</td>
  </tr>
  <tr>
    <td>[politician, actor, television actor...]</td>
    <td>[Bachelor of Arts, Master of International Affairs...]</td>
    <td>3</td>
    <td>2018</td>
  </tr>
</table>
 
<br>

# <a name="description"></a> **Descriptitve analysis**: An overview of the dataset

The dataset, as said before, was reduced to have an optimal analysis. Let's take a look at what it contains keeping in mind the two pillar questions around which this study is conducted:


<center><span style="color:DarkSlateBlue"><font size="5">Do women speak more in general after the movement?</font></span></center>

<center><span style="color:DarkSlateBlue"><font size="5">Has the representation of women's occupations changed after #MeToo?</font></span></center>

<br>

{% include imagetextright.html figname="Percentage_of_speakers_by_gender_and_by_period.html" title="Counting the quotes published for each gender" description="> The voice in the newspapers is much more given to men than to women (about 80% against 20%) which is similar to the figures published in 2015. A slight evolution of the rate of women's speech appears between the periods but it remains to be investigated." %}

<br>

{% include imagetextleft.html image_path="D-occ-female.png" title="Looking at the occupation of women quoted" description=">It is observed that the most talked about women are politicians, lawyer, writer, university teacher. The distribution is however highly skewed indicating a huge asymmetry in the representation of occupations in newspapers" %}  

<br>

After this short description of the dataset, let's get down to business!

# <a name="obsstudy"></a> **Matched Observational Study**: The ideal setting to a causal analysis

<div style="text-align: justify"> Let's recall the problematic around the analysis: </div>
 
 <br>
 
 <center><span style="color:DarkSlateBlue"><font size="5.2"><i>Has the MeToo movement affected the representation of women in the newspapers?</i></font></span></center>
 
 <br>
 
<div style="text-align: justify">Since the quotebank dataset is a found dataset, and not a created experiment, it is appropriate to call its analysis an observational study. With the reduced dataset containing only speakers with enough known characteristics, the following analysis is conducted: a <strong>matched observational study</strong>. This means that the dataset is reduced and cut in two in a way that for every speaker of a certain gender quoted before #MeToo thus belonging to the before #MeToo dataset (i.e., before October 2017), a very similar speaker (or the same one if this one is quoted after MeToo) of the same gender belongs to the new dataset of after #MeToo quotes. Similarity is measured by the degree of similitude of the features obtained on the speakers. Any pre #MeToo speaker that is not paired with a post #MeToo counterpart (and vice versa) is thus removed from the dataset. Therefore, the 'before' dataset contains speakers extremely similar the the 'after' dataset i.e. the speakers have the same characteristics. The two new datasets can be approximated to be the same in term of the speakers each contains and thus can be properly compared with no risk of confounders interfering with the causality.</div>

# <a name="first"></a> **First Question of the Study**: Do women speak more in general after the movement?

<div style="text-align: justify">Previously, it was observed that significantly more men were quoted at any period of time. However, the graph below shows when the median number of quotes said per person is counted, women dominate, both before and after #MeToo with an intensification of the male-female difference after the movement. Nevertheless, this increase is a general trend that can be found for both genders and nothing can be concluded about the role played by the movement in favor of this female rule. So while few women are quoted compared to men, those who are will be listened to much more than the average man quoted. What prevails is the idea that a woman must be much more important and listened to in order to appear in the newspapers.</div>


{% include Impact_meetoo_median_quotes_occurrences_gender.html %}


<div style="text-align: justify">Moreover, after some statistical test (<a href="https://statistics.laerd.com/spss-tutorials/wilcoxon-signed-rank-test-using-spss-statistics.php">wilcoxon signed rank test</a>) it was found that for any pairing of speakers before and after the movement, the probability of a speaker after #MeToo to have more quotes published than the speaker before #MeToo is of 0.56 for male and 0.57 for female. Thus, it can be concluded that, in general, speakers after the movement speak more than speakers before. However, even if this phenomenon seems to be a little bit more pronounced for women, the same trend is followed by both genders, with small effects. It is possible that this analysis is too general, so we decided to focus only on certain occupations for the rest of the analysis. Thus, we will analyze if the profile of the female speakers has changed i.e. whether the professions represented have differed post-Metoo, and once again we will compare this evolution with male speakers.</div>

# <a name="first"></a> **Second Question of the Study**: Has the representation of women's occupations changed after #MeToo?

## <a name="prof"></a> **Professions representation in the matched observational sutdy dataset**

<div style="text-align: justify">An important feature that was added to the dataset are the occupation categories. Since there were over 900 occupations in the dataset, we created 40 categories to group them together and allow for a simplified assessment of the representation of occupations in the journals. For example, a person with the category "Teaching & Education" could be an academic administrator, a teacher, a Ph.D. student, a faculty member, a guidance counselor etc. With the balanced dataset, a lot of speakers have been removed and the ones remaining have the same characteristics before and after #MeToo in the globality. Thus the following wordcloud shows the male and female's categories of occupations displayed in the balanced datased both before and after #MeToo as they coincide in terms of charatceristics. The size of the font is proportional to the frequency with which the category appears.</div>

<img src="wordcloud.png" alt="">

<div style="text-align: justify">The most represented categories of occupations are quite similar for the men and women, before and after metoo, with teaching, government staying the most represented ones. Keep in mind that this wordcloud represents the words in term of proportion between them, meaning that the teaching category for men has not the same occurence as the teaching category for women, even if on the wordcloud, the word teaching has the same size for both gender.</div>

<br>


 <div style="text-align: justify"><strong>For the next analysis, we focus only on the most reprensented categories of occupations for both genders.</strong></div>


<br>
























## <a name="targ"></a> **Targeted matching according to occupations**

<div style="text-align: justify">Here again, the dataset is reduced and cut in two in a way that for every speaker of a certain gender and a given category of occupation quoted before #MeToo, a very similar speaker of the same gender and category of occupation belongs to the new dataset of after #MeToo quotes (for more technical see the <a href="https://github.com/epfl-ada/ada-2021-project-adamn">code</a> we did on the matching). It is now possible to analyse if some categories of occupations are more represented after #MeToo.</div>

<br>

### <a name="visu"></a> **Visualisation of the evolution of the gender's occupation's around the movement**

<div style="text-align: justify">The graph below shows the median number of occurences of quotes and number of quotes said according to the gender and the category. We can first notice that both genders show an increase for the medians after #MeToo. Concerning the number of quotations, we observe a higher median for male than for female for the categories Teaching and Government (only after #MeToo) and Historian (before and after #MeToo). For the number of occurrences, the median is higher for female than for male in all cases except for the Historian category. This could indicate that even if the number of male speakers is higher than the number of female speakers, in most cases a single female speaker will have more quotations occurrences than a man, the quotation of a female seems to be  more relayed.</div>

<br>

<img src="O-med-occ-occurence-female.png" alt="">

<br>

<div style="text-align: justify"><strong>Let's look at the ratio of these medians between after #MeToo and before to better visualize how each category has really evolved over the period of the movement.</strong></div>

<img src="O-ratio.png" alt="">

<div style="text-align: justify">Thus, after the assessment that the number of quotations and of occurrences have indeed increased after #MeToo for both genders, we can now clearly observe the following evolution for the two genders: a higher ratio After/Before for female than for male except for the following cases:</div>

<br>

- For the number of quotes: Teaching, Government, Scientist, Media
- For the number of occurrences: Historian


<br>

<div style="text-align: justify">It is interesting to observe that the female evolution is more important than the male's one in most of the cases and particularly in the number of occurrences. This number of occurrences underlies the representation and the importance given to a quote. This could let us think that the representation of women in newspapers has indeed increased. </div>





### <a name="stat"></a> **Supporting statistical tests for advanced analysis**



Among all the significant results for occupation/gender pairs, , those with the highest effect size are observed for female speakers for both number of quotations and number of occurrences.  For the number of quotes, we obtain a significant difference in the median combined with a common language effect size greater than 0.58 for female speakers working in government, social science, law, and for female historians. This is also observed for women from the non-scientist group, as well as for those in the non-teaching and education group. Looking at the number of occurrences, the highest effect sizes are observed for women working in government or in the legal field.

We can conclude that:
- Again, all speakers speak more after than before the movement, with the exception of women in the media and journalism field.
- However, although men also speak more after the MeToo movement, it can be said that their increase in speech is less compared to women: indeed, the largest effects are observed for women.
- Women speak more after the MeToo movement, but no category really stands out more than others, with the exception of women involved in government.
- Even though women speakers working in Law have a significant difference in median number of quotes and occurrences, and have one of the highest effect sizes in both cases, we cannot conclude anything about them, since we have seen that the 95% confidence intervals of the median for these women is huge.
- However, women working in government seem to have changed the most after the movement. Indeed, their ratio of number of quotes after to number of quotes before is still lower than that of men, but their total number of occurrences has almost doubled! Moreover, their evolution is much more visible than for all other women not working in government.

<img src="O-government.png" alt="">







# <a name="conclu"></a> **Conclusion of the Analysis**: Has the #MeToo movement had an impact on women's voices and representation in the newspapers?


In 2020, the number of women quoted in newspapers does not even reach 25%. We are still far from parity. However, when a woman is a speaker, she tends to have a higher number of quotes as well as a higher number of occurrences than a man: the floor seems to be given to women only if they are really important. Otherwise, the floor is preferentially given to men. Our study shows that the number of quotes, as well as the number of occurrences linked to them, increased after the #MeToo movement for all speakers, men and women alike. All actors gain visibility over time: this may be due simply to the increase in digital news platforms and the ever faster sharing of information, but further research into the causes should be conducted. However, it seems that the relative increase is greater for women in most categories of occupations, especially in terms of occurrences. One significant difference is that women politicians seem to have gained a lot in terms of visibility and credibility. Indeed, compared to women who are not politicians, their evolution is much greater. In particular, their median total number of occurrences per woman has almost doubled after MeToo! This phenomenon may be the result of both the MeToo movement and the 2016 presidential election, in which the official Democratic Party candidate was a woman, Hilary Clinton, for the first time in history. This sequence of events has led to an increase in the credibility of women politicians. However, there is still a long way to go to achieve parity in media coverage, and the effect of MeToo on the representation of women in the newspapers is not as high as expected, but it is still a good start...




