---
layout: default
---
# A few data on women's mis-representation in the media

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


# <a name="context"></a> **Context**: The #MeToo movement 

<div style="text-align: justify"> In 2006, Tarana Burke, activist and sexual assault survivor, creates the MeToo movement in support to all women victims of crimes of sexual nature. It is only in October 2017, when more than 80 women in the film industry made sexual abuse allegations against film producer Harvey Weinstein, that the MeToo movement re-emerged. The actress Alyssa Milano is the one who reignited the movement by encouraging victims of sexual harassment and assault to come forward using the hashtag #MeToo as a status update on Twitter. With the goal of raising awareness of sexual misconduct, empowering survivors to speak out, helping them heal as a community by not feeling alone in this battle, and bringing them justice, the MeToo movement has spread around the world, showing the reality and magnitude of sexual abuse against women.  </div>

<br>

<div style="text-align: justify"> </div> The re apparition of this movement 

INTRODUIRE ET PARLER DU GRAPHE

<img src="D-lex.png" alt="">

<div style="text-align: justify">Moreover, and most importantly, by inviting thousands of women to come out of the shadows, to protest against such violence, to make themselves heard and to demand justice, these survivors have given the movement an even more important dimension in the fight for gender equality. Indeed, they have empowered the voices of women all around the world.  </div>
<br> 
<div style="text-align: justify"><span style="color:Red"><strong>It is hoped to find in this analysis, that this empowerment will reverberate through to the newspapers, where women's voices would be better heard, represented, diversified and accepted.</strong></span>  </div>


# <a name="quotebank"></a> **The Quotebank Dataset**: A goldmine of information on the role of women in the media

DIRE QUE AU DATASET ON A RAJOUTÉ LES OCCUPATIONS académic degree
METTRE UNE QUOTES.

<div style="text-align: justify"> 178 million quotations along with its speakers extracted from hundreds of english articles from 2015 to 2020 together in one open corpus; That's the <a name="qtdata" href="https://dlab.epfl.ch/people/west/pub/Vaucher-Spitz-Catasta-West_WSDM-21.pdf">QuoteBank Dataset</a>. A goldmine of information on the subjects, personnalities, ethnicities, genders, careers etcetera represented in the newspaper and displayed to a target audience in the last five years. Off the NUMBER of quotations and NUMBER of known speakers retrieved from the dataset, the analysis was conducted on NUMBER of quotations said by NUMBER of speakers. Indeed, the dataset being too important and full of unknown speaker caracteritsics, data processing has been done retrieving only speakers with known CECI et CELA for a much more relevant and reliable dataset applicable to </div> [matched observational studies](#obsstudy). 


# <a name="description"></a> **Descriptitve analysis**: An overview of the dataset

INTRODUIRE 2 Q : Est ce que les femmes parlent plus en générale après metoo? Est ce que la rpz des femmes à changer en termes de leur occupations?

{% include test.html image_path="D-perc-quot-genders-period.png" title="Title" description="> Description" %}  

CONLCU: bcp plus d'hommes en général (80% 20%) => similaire à 2015 et une légère évolution du taux de paroles de la femme qui reste à investiger (est ce metoo ou autres). Occupations: les femmes qui parlent e-le plus politicienne lawyer writer, university teacher distribution skewed

# <a name="obsstudy"></a> **Matched Observational Study**: The ideal setting to a causal analysis

<div style="text-align: justify"> Let's recall the problematic around the analysis: </div>
 
 <br>
 
 <center><span style="color:Red"><font size="5.2"><i>Has the MeToo movement affect the representation of women in the newspapers?</i></font></span></center>
 
 <br>
 
<div style="text-align: justify">Since the quotebank dataset is a found dataset, and not a created experiment, it is appropriate to call its analysis an observational study. With the reduced dataset containing only speakers with enough known characteristics, the following two analysis are conducted. The first is only a <strong>description of the dataset</strong>. The second is a <strong>matched observational study</strong>. This means that the dataset is reduced and cut in two in a way that for every speaker quoted before #MeToo thus belonging to the before #MeToo dataset (i.e., before October 2017), a very similar speaker (or the same one if this one is quoted after MeToo) belongs to the new dataset of after #MeToo quotes. Similarity is measured by the degree of similitude of the features obtained on the speakers (SET CHARACTER). Any pre #MeToo speaker that is not paired with a post #MeToo counterpart (and vice versa) is thus removed from the dataset. Therefore, the 'before' dataset contains speakers extremely similar the the 'after' dataset i.e. the speakers have the same characteristics. The two new datsets can be approximated to be the same in term of the speakers it contains and thus can be properly compared with no risk of confounders interfering with the causality.</div>

PARLER DES GENDERS
 
 
# <a name="first"></a> **First Question of the Study**: Do women speak more in general after the movement?

GRAPHE MEDIANE : on avait vu qu'il y avait bcp plus d'hommes qui parlent cependant quand on regarde le nombre de citation par speaker les femmes parlent plus que ce soit avant ou après. MAIS après la différence est intensifiée. CEPENDANT tout le monde parle plus après metoo. MEME tendance entre nombre de quotes et nombre d'occurence donc a partir de maintenant l'analyse ne représentera que le nombre de quotes as they follow the same trend.

{% include occupation.html %}


MOREOVER, after some stattiscal test (wilcoxon signed rank test lien).For any pairing of speakers befre and after the movment, the proba of the speaker after to ahev more quotes than the speaker before is 0.56 for male and 0.57 for female. Donc Thus, we conclude that in general speakers after #MeToo speaks more than speakers before #MeToo. However, even if this phenomenon seems to be a little bit more pronounced for women, we osberve the same trend for both gender, with small effect sizes. We think that our analysis might be too general, so we decide to focus on certain occupations for the rest of the analysis. We will analyze if the profile of the female speakers has changed: whether the professions represented have differed post-Metoo, and once again we will compare this evolution with male speakers.



# <a name="first"></a> **Second Question of the Study**: Has the representation of women's occupations changed after #MeToo

## Professions representation in the matched observational sutdy dataset

PARLER DES catégorie OCCUPATIONS METTRE DES EXEMPLES de quelles occupation dans quel catégories.

voici occupation de nouveau dataset les plus représentés. Un seul graphe par genre sur le balanced dataset
What are the main categories of occupations represneted in the news among men and women speakers.

GRAPHE JEANNETTE

Parler de proportion sur les graphes de jeannette.

## Targetted matching according to occupations

Analyse if some categoreis of occupation are more represented. 


Here again, the dataset is reduced and cut in two in a way that for every speaker of a given category of occupation quoted before #MeToo, a very similar speaker of the same category of occupation belongs to the new dataset of after #MeToo quotes (for more technical detail lien du notebook). 


GRAPHE: median of the number of quotes by occupation par gender
dessus: inspirer des commentaires. Dire que ce soit chez hommes ou femme on observe augmentation de la médiane de nombre de quotation après pour les deux genres. Et c'est pour toute les occupations on observe ca. Onobserve higher lédiane en générale chez femme sauf pour certaines exception (voir texte julie seulement quotation et médiane). EN évaluant évolution chez lees deux ca a plus évolué chez les femmes sauf pour teaching government scientist et media ou il y a plus grandes d'occupations de la médiane pour les quotes chez les hommes que chez les femmes. faut further analysis pour assess augmentation.
Pour l'instant a part exception rpz des femmes a augmenter a investiguer avec des test stat.


EN FAISANT DES TEST STAT on trouve que les différences avant après pour chaque genre et chaque occupation sont significcatives SAUF pour les fmemes media&journalisme et on trouve que leffet les plus grand c'est pour les historienne femme.









