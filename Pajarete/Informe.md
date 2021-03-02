Characterization of the microbiota from two vineyards at ‘Valle del
Huasco’ in the northern Chile and inference of its metabolic pathways
================
Benjamín Valderrama,
2020

<style>
body {
text-align: justify}
</style>

<font size="5"> **Resume** </font>

The microbiota associated with wine production can affect the flavor and
aroma of the end product, therefore, its study can provide important
tools for improving the wine quality. In this work I used the V4 region
of the marker gen 16S rRNA to characterize the microbiota associated
with the production chain of two vineyards at ‘Valle del Huasco’. Then,
I identify taxonomic signatures present in the vineyards with LefSe and
used Piphillin to infere its metabolic pathways. Here I report taxonomic
signatures with highly specific presence in the vineyards. Some of them
had never been described before, while others, like Lactobaillales, are
widely recognized by their metabolic products and its capability to
modify wine’s organoleptic properties. Anyway, prior to made strong
conclusions about the effects of the microbiota in the production of the
Pajarete, the bioinformatic approximation here exposed has to be
complemented with experimental work. As consequence, this report
represents the first step to explore the commercial worth of a wine with
appelation of origin, and, therefore, unique in the world.

<font size="5"> **Introduction** </font>

The usage of microorganisms in the production of human food has been
well studied since long ago (Ozen & Dinleyici, 2015). Nowadays, with
next generation sequencing technologies (NGS), we have much more refined
knowledge of its effects on our foods and drinks. In the case of red
wine, the microbiota associated with its production chain is essential
for fermentation of the most, and has consequences for relevant
properties of the end product, like its flavor and aroma (Sirén, Mak,
Fischer, Hansen, & Gilbert, 2019). Those features depends on volatile
molecules present on it, which in turn are products of the metabolic
activity of the microbiota(Parker, Capone, Francis, & Herderich, 2018).
This evidence set the interest to study the microorganisms community and
comprehend its relationship with the productive process, either to
manipulate and potentiate wine’s organoleptic properties or to enhance
its regionalized origin; being both scenarios capable increase its
market value (Sirén et al., 2019; Varela & Borneman, 2017). As
consequence, because of a wider knowledge of the microbiota associated
with the production chain, huge business opportunities can be opened.

In particular, the ‘pajarete’ is a sweet red wine which is produced,
commercialized and consumed in small quantities (Castro et al., 2016).
This wine has appellation of origin at northern Chile since 1953; a very
singular situation within alcoholic drinks, being only preceded by the
chilean ‘Pisco’ (Lacoste et al., 2016). This acknowledgment given almost
a century ago, and its consequent outstanding position among other
drinks, strongly contrast with its almost unnoticed condition in
researching fields. Indeed, there is only one paper about ‘pajarete’.
Because that publication only discuss historical aspects of the
‘pajarete’ wine (Castro et al., 2016), all data presented herein must
be considered as a first approximation to the microbiota associated with
the production of a previously unexplored product through bioinformatic
methods.

Next generation sequencing methods has been routinely used to explore
the communities of microorganisms living in diverse environments and
food products. One common strategy to identify this microorganisms is
thorugh the sequenciation of the marker gen 16S rRNA. Nevertheless, this
technique cannot allow researchers to straightforward identify the
metabolic activities of the community. In order to do that, it has been
suggested to integrate different ‘omic’ strategies (metagenomics,
transcriptomics, metabolomics, etc), but because of its high costs, they
usually are very restrictive (Knight et al., 2018). Although indirect, a
more economical approximation is the inference of microbiota’s metabolic
pathways from the marker gen using statistical tools, sucha as Piphilin
(Iwai et al., 2016), which was used in this work.

The relevance of the microbiota associated with wine’s production and
the almost null knowledge we have about the ‘pajarete’, set the interest
of the producers and researchers to inquire the composition of those
communities, the metabolic pathways they bear and its consequences on
wine’s propierties that can modify its value in the market. To do that,
and in consideration of the exploratory nature of the analysis presented
here, NGS technologies were used on the V4 region of the 16S rRNA marker
gene, with the following inference of metabolic pathways present in the
microbiota of two different producers of ‘pajarete’ to get insights in
this unexplored territory.

<font size="5"> **Objectives** </font>

The general objective of this work is the characterization of the
microbiota associated with the ‘pajarete’ produced in two artisan
vineyards located in ‘Valle del Huasco’ in the northern Chile

In particular, it is expected to get insights about the composition of
this community through the analysis of metagenomic data produced with
NGS methods. Then, to analyze taxonomic features in the production
chains used by the two vineyards and, finally, to predict the metabolic
pathways beared by both communities.

<font size="5"> **Material and methods** </font>

  - **Biological samples :**

The samples herein used come from two artisan vineyards which produce
‘pajarete’ at ‘Valle del Huasco’. Because of their desire to keep its
production process in confidence, from now are referred as JF y VG. The
V4 region of the 16S rRNA marker gene was amplified and sequenciated
with 515F and 806R primers with Illumina MiSeq technollogy. In both
vineyards, samples were collected in four different stages in the
respective production chain, being them: “Before grinding” (JF1 and
VG1), “After pressing” (JF4 and VG3), “Before the fermentation stop”
(JF5 y VG4) and “After the fermentation stop” (JF6 and VG5).
Nevertheless, the sampling process was made two month before the author
received the data, and therefore was not involved on it.

  - **Workflow for metagenomic data analysis :**

Metagenomic data was filtered acording to its quality. Qualified reads
were then assigned to a taxonomic classification using dada2 algorithm
(Callahan et al., 2016) and Silva database version 138.1 (Quast et al.,
2013; Yilmaz et al., 2014). Then, two filters were applied to reads; the
first filter was “supervised” and aims to remove reads assigned as
“uncharacterized” at the phylum level, as well as reads considered as
mitochondria, chloroplast or eukaryotic life forms. The second filter
was “unsepervised” and was applied to discard reads within any phylum
that has just one sinlge read. Then all samples were normalized by sum
of squares with the vegan R package. After that, alpha diversity was
calculated and a t-test was conducted to identify differences between
vineyards. Later, beta diversity was calculated and PERMANOVA was then
applied. Finally, taxonomic composition of samples were inquire by
analyze its relative abundances at phylum and family level.

  - **Taxonomic features associated with each producers and metabolic
    pathways inference :**

LefSe algorithm (Segata et al., 2011), free available in Dr. Huttenhower
website, was used to identify taxonomic features in both production
processes. This algorithm applies Kruskal-Wallis test (alpha = 0,05) and
the subsequent Wilcoxon test (alfa = 0,05). Taxonomic features were
identified given a LDA threshold score of 2.0. After that, Piphillin
(Iwai et al., 2016) was used with data stored at Kyoto Encyclopedia of
Genes and Genomes (KEGG) (Kanehisa & Goto, 2000) to infer functional
metabolic pathways within microbial communities of both ‘pajarete’
producers. Multiple t-Test with Benjamini, Krieger y Yekutieli False
Discovery Rate (Q = 1%) were conducted in order to identify pathways
strongly associated with each vineyard.

<font size="5"> **Results** </font>

  - **Relative abundance of the bacterial community within JF and VG
    vineyards, by phylum:**

To know the composition of the microbiota associated with this two
producers of ‘pajarete’, relative abundances of the phyla present in the
communities were plotted. The results are shown in Figure 1. Each phylum
has a color, and each bar represents a different sample, properly
identified by its name on the X axis, and its percentage value on the Y
axis.

*Firmicutes* are predominant in samples JF1 and VG1, which correspond to
stages before the processing of the most. Although *Firmicutes*
representation within the community is lower in other samples, those
microbiotas are still constituted almost entirely by *Firmicutes* and
*Proteobacteria*

Fig 1: Barplot of relative abundances of the bacterial community within
JF and VG vineyards, by phylum:

![Alt
text](https://github.com/Benjamin-Valderrama/Microbiome_Portfolio/blob/master/Pajarete/Resultados/abund_phylum.png)

(C:/Users/Acer/Documents/Microbiome_Portfolio/Pajarete/Resultados/abund_phylum.png)

  - **Relative abundance of the bacterial community within JF and VG
    vineyards, by family:**

Additionally, the relative abundances of the microbiota associated with
the two producers was inquire at family level of the taxonomy hierarchy.
Results are shown in Figure 2. Each of the 12 most abundant families has
a color. Also, reads that were not assign to any family (NA in the
figure) were represented in dark gray. The contribution of all the other
families is represented in light gray. Each bar represents a different
sample, properly identified by its name on the X axis, and its
percentage value on the Y axis.

Samples JF1 and VG1, which correspond to stages before the processing of
the most, shown that *Lactobacillales* is the prevalent family. In the
other samples, the 12 most abundant families represent around 25 to 75%
of those communities.

Fig 2: Barplot of relative abundances of the bacterial community within
JF and VG vineyards, by family:

![Alt
text](C:/Users/Acer/Documents/Microbiome_Portfolio/Pajarete/Resultados/abund_familia.png)

  - **Alpha diversity of the microbiota associated in JF and VG
    ‘pajarete’ producers**

Figure 3 shows alpha diversities of the two ‘pajarete’ producers. Three
diferent metrics were used: Observed diversity, in A; chao1 index, in B
and Shannon diversity in C. Two tiled t-Test were conducted to identify
differences between producers: in A, (t6 = -2.46, P = 0,054); in B, (t6
= -2.46, P = 0,054) and in C, (t6 = 0.62, P = 0.56). As consequence, the
observed differences are not statistically significant for any metric.
Samples showed in Red comes from JF producer, and those in Green comes
from VG.

Fig 3: Alpha diversity of the communities present in JF and VG vineyards
mesured as Observed diversity, Chao1 index and Shannon diversity

![Alt
text](C:/Users/Acer/Documents/Microbiome_Portfolio/Pajarete/Resultados/alpha_div_todas_las_muestras.png)

Figure 4 shows alpha diversities of the producers after removal of JF1
and VG1 samples, both corresponding to “Before grinding” phase of the
production process. The same metrics as in the previous figure were used
here: Observed diversity, in A; Chao1 index, in B; and Shannon diversity
in C. Two tiled t-Test were conducted to identify differences between
producers: in A, (t4 = -5.13, P = 0,0089); in B, (t4 = -5.14, P =
0,0089) and in C, (t4 = 1.27, P = 0.29). As consequence, the differences
between metrics shown in A and B are now statistically significant, but
no for C.

Fig 4: Alpha diversity of the communities present in JF and VG vineyards
after the removal of “Before grinding” samples, mesured as Observed
diversity, Chao1 index and Shannon diversity

![Alt
text](C:/Users/Acer/Documents/Microbiome_Portfolio/Pajarete/Resultados/alpha_div_solo_prod.png)

  - **Beta diversity of the microbiota associated in JF and VG
    ‘pajarete’ producers**

The Figure 5 shows a MDS plot with beta diversity results. UNIFRAC and
Bray-Curtis metrics were conducted followed by its subsequent PERMANOVA
(F1,6 = 2,16; P = 0,15 y F1,6 = 0,24; P = 0,089, respectively). As seen,
observed difference were not statistically significant. Nevertheless, it
is a trend showed by data in which, regardless the phase of the
production chain looked at, samples from the same producer seems to be
more similar to each other than samples from the same phase, but from
the other vineyard. This is true with the exception of those samples
corresponding to “Before grinding” phase.

On the graph, each phase of the production chain has its own shape.
Also, Red points represent samples from JF, while Green, samples from
VG.

Fig 5: Beta diversity for samples of two vineyards measured with UNIFRAC
and Bray-Curtis methods:

![Alt
text](C:/Users/Acer/Documents/Microbiome_Portfolio/Pajarete/Resultados/PCoA_b-diversity_etapas.png)

  - **Taxonomic features associated with each production processes:**

With the LefSe service, available in the web, the taxonomic features
present in samples from the two ‘pajarete producers’ were identified.
Figure 6 shows the results of this identification at the Family level in
the taxonomic hierarchy. With red were signaled those samples collected
from JF, while those from VG are showed in green

Fig 6: Specific taxonomic features identified in each of both production
processes; JF and VG.

![Alt
text](C:/Users/Acer/Documents/Microbiome_Portfolio/Pajarete/Resultados/Galaxy42.png)

Also with LefSe, the phylogenetic relationships of bacteira founded
within samples of each producer of wine. This result was depicted in
Figure 7. The figure shows in red those samples collected from JF and in
green those from VG. Also, the legend shows to which taxonomic feature
correspond each of the depicted areas within the phylogenetic tree.

Fig 7:Phylogenetic relationships between bacteria associated with each
of both production processes; JF and VG.

![Alt
text](C:/Users/Acer/Documents/Microbiome_Portfolio/Pajarete/Resultados/Galaxy43.png)

  - **Metabolic pathways inference:**

Using Piphillin, a web algorithm available in the web, the metabolic
pathways harbored by microbial communities from both producers were
inferred. Figure 8 shows pathways that were found to be most abundant in
JF samples, while in green are shown those for VG. The table 1, within
the supplemental material section, shows the p-values obtained from each
of the multiple t-test with False Discovery Rate of Benjamini, Krieger y
Yekutieli that were conducted.

Fig 8: Metabolic pathways inferred from samples collected within JF and
VG production chains. This pathways were inferred from the 16S rRNA
sampled data.

![Alt
text](C:/Users/Acer/Documents/Microbiome_Portfolio/Pajarete/Resultados/Pathways_clean.png)

<font size="5"> **Discussion** </font>

Because of the lack of previous literature dedicated to analyze the
microbial community associated to the production of the ‘pajarete’, the
results presented here, pointing the prevalence of *Firmicutes* and the
later change in the composition of the biota, are new. Also, its causes
can not be determined from the analysis conducted during this work.
Nevertheless, a plausible explanation of this changes in the relative
abundances is due to the different conditions the most is subject along
the processing stages. Changes in temperature and pressure during the
processing of the most can favor different phyla and/or families in each
step, and could lead to the changing representation of those taxonomies
within the samples.

Additionally, is worth to mention that the decision to analyze relative
abundances of the collected samples just as deep as the family level of
the hierarchy was due to the final number of reads for each sample. Some
of them can not meet the usual standards for number of reads that can be
seen in this type of experiments. As consequence, bacteria from some
genus or species that are present in the community, can be
underrepresented within the sample.

Results for alpha diversities are interesting. After remove those
samples corresponding to “Before grinding” stages for both producers,
and conduct the analysis to compare the diversity values, the effect
size (difference) between metrics for two producers become acute. It is
consistent with the results exposed in the beta diversity analysis
discussed below.

As said, the analysis of beta diversities shows a trend on which samples
from each producer tend to be more similar within them, than they are
with samples from the other producer even if it was collected at the
same stage of the production process. However, this is not the case for
samples corresponding to “Before grinding” stage, where they tend to be
much more similar within them than with other samples, no matter the
producer of which they come from. This suggest that before the
production process used in each vineyard, all communities tend to be
closely related in terms of their diversities, but along the processing
chain of the most, and due to different conditions used by each
vineyard, communities tend to differentiate between them and come to
cluster by its producer. Given the above, and even in consideration that
differences are not statistically significant, the trend previously
depicted rise the worry to increase the number of replicates and then
conduct the same analysis

By the end of september 2020, there are no papers about the microbiota
associated with the production of ‘pajarete’ in any of the scientific
literature research engines. Nevertheless, reading the available
literature which discuss the microbiota of other wines, it is
interesting the reported presence of *Lactobacillaes* microbes, also
noticed in ‘pajarete’, which are repeatedly discussed as important
malolactic fermenters (Lonvaud-Funel, 1999; Reguant & Bordons, 2003),
and therefore, play an important role in determining wine’s quality
(Ilabaca, Jara, & Romero, 2014). Although *Alphaproteobacterias* were
identified within the studied communities, its presence is not something
to worry about, because non of the three genera known to be producers of
acetic acid (Bartowsky & Henschke, 2008) were present in the samples.
Other relevant aspect of the bacterial composition in the samples, is
the presence of taxonomic features that has never been described before
in wine’s literature. It opens the door for the exploration of the
consequence of its presences in the produced ‘pajarete’. This is the
case for *Muribaculaceae* and *Pectobactericeae* in VG vineyard, and
*Planococcaceae* in JF.

The enrichment in the metabolic pathways associated with valine, leucine
and isoleucine degradation in samples collected from JF is consistent
with previous reports. The supplementation of low-linoleic-acid mosts
with those aminoacids enhance the production of volatile compounds, like
alcohol and others associated with wine’s flavor and aroma (Liu, Yu, Li,
Duan, & Yan, 2018). In Liu’s paper, it was also concluded that linoleic
acid can regulate the expression of genes involved in the production of
volatile molecules within wines that were supplemented with this acid.
Additionally, other research suggests that some unsaturated fatty acids
-also detected as statistically significant in this study- are
determinants in the final flavor and aroma of the produced wine, and,
also, can affect the fermentative performance of *Saccharomyces
cerevisiae* (Liu, Duan, & Yan, 2019).

Some pathways of the nitrogen metabolism, also enriched in samples from
JF vineyard, had been associated with an increase in the concentration
of metabolites produced during the alcoholic and malolactic
fermentations (Lytra, Miot-Sertier, Moine, Coulon, & Barbe, 2020), being
the last consistent with the detection of high presence of
*Lactobacillales* within JF samples. These metabolites had been
characterized as relevant for determining amoratic properties of the
wine (Lytra et al., 2020). Also, the presence of geraniol and genaric
acid has been reported as relevant for the same organoleptic properties
named above, in different kinds of red and white italian wines (De
Lorenzis, Squadrito, Brancadoro, & Scienza, 2015). Finally, other
relevant result herein exposed is the pathway for benzyl alcohol and
other benzoate derivatives, which confer fruity and floral flavors to
wines (Martin et al., 2016).

Finally, it is necessary to make explicit an assumption used in the
statistical analysis done in this report. All statistical test were made
with samples from different stages along the production process of the
‘pajarete’. Because of each stage has just one replicate, it was
impossible to know the effect of each step of the process in the
observed differences when doing diversity, community composition or
metabolic pathways statistical analysis. The decision to group samples
from different steps comes from the assumption that all of them can
reflect, globally, the entire process of production used by each
vineyard. Although useful in term of statistical analysis, this
assumption implies that the temporal structure which underlies the
samples was deliberately ignored. Therefore, factors that without doubt
affect the bacterial community studied, like time and the temperature or
pressure conditions in which the most is processed to produce wine, were
laid by side and not considered when trying to explain the observed
differences. With all issues above discussed, results here exposed must
be carefully analyzed and considered as a first approximation to this
unexplored field.

<font size="5"> **Final thoughts** </font>

Without doubt it is desirable to integrate metagenomic studies with
metatranscriptomic and metabolomic approaches. Nevertheless, due to its
high cost, the present work shows the indirect prediction of metabolic
pathways from the 16S rRNA marker gene. In consequence, it is relevant
to conduct empirical work to test some hypothesis that emerged after
this bioinformatic workflow. Interesting hypothesis to further explore
are: which role plays this bacteria never described in wine samples
before? Does metabolic pathways herein inferred correlate or explain
some properties of the end product? What is the effect of the yeast
involved in this process?

Additionally, an increase in the number of samples in each step of the
production chain will allow to gain more deep insights about the inner
dynamics of the bacterial community. Its composition, here analyzed in
terms of relative abundances, changes along the production process,
probably due to pressure and temperature conditions which it cross
trough. Also, analysis of the community diversity shows a trend of
differentiation, on which samples tend to follow a divergence process
which end in major similarity within each producer that the observed
similarity within production step.

Finally, it is interesting to mention that ‘pajarete’, a wine with
appellation of origin and an historical background, was almost neglected
in terms of its biological determinants for the production process and
the end product. This is an opportunity to further explore the microbial
community associated with this wine and, then, use this knowledge to
enhance the organoleptic properties of a beverage that can only be
produced here in Chile, and therefore, counts with high comparative
advantages in the world market.

<font size="5"> **Reference** </font>

<div id="refs" class="references">

<div id="ref-Bartowsky2008">

Bartowsky, E. J., & Henschke, P. A. (2008). Acetic acid bacteria
spoilage of bottled red wine-a review.

</div>

<div id="ref-Callahan2016">

Callahan, B. J., McMurdie, P. J., Rosen, M. J., Han, A. W., Johnson, A.
J. A., & Holmes, S. P. (2016). DADA2: High-resolution sample inference
from illumina amplicon data. *Nature Methods*, *13*(7), 581–583. Nature
Publishing Group.

</div>

<div id="ref-Castro2016">

Castro, A., Pszczólkowski, P., Mujica, F., Lacoste, P., Núñez, E.,
Cofré, C., Adunka, M. L., et al. (2016). El pajarete de huasco y elqui
(chile): Historia de un vino escogido. *Idesia (Arica)*, *34*(ahead),
0–0. SciELO Comision Nacional de Investigacion Cientifica Y
Tecnologica (CONICYT).

</div>

<div id="ref-DeLorenzis2015">

De Lorenzis, G., Squadrito, M., Brancadoro, L., & Scienza, A. (2015).
Zibibbo nero characterization, a red-wine grape revertant of muscat of
alexandria. *Molecular Biotechnology*, *57*(3), 265–274. Humana Press
Inc.

</div>

<div id="ref-Ilabaca2014">

Ilabaca, C., Jara, C., & Romero, J. (2014). The rapid identification of
lactic acid bacteria present in chilean winemaking processes using
culture-independent analysis. *Annals of Microbiology*, *64*(4),
1857–1859. Springer Verlag.

</div>

<div id="ref-Iwai2016">

Iwai, S., Weinmaier, T., Schmidt, B. L., Albertson, D. G., Poloso, N.
J., Dabbagh, K., & DeSantis, T. Z. (2016). Piphillin: Improved
prediction of metagenomic content by direct inference from human
microbiomes. (Z. He, Ed.)*PLOS ONE*, *11*(11), e0166104. Public Library
of Science.

</div>

<div id="ref-Kanehisa2000">

Kanehisa, M., & Goto, S. (2000, January). KEGG: Kyoto encyclopedia of
genes and genomes. Oxford University Press. Retrieved from
<https://pubmed-ncbi-nlm-nih-gov.pucdechile.idm.oclc.org/10592173/>

</div>

<div id="ref-Knight2018">

Knight, R., Vrbanac, A., Taylor, B. C., Aksenov, A., Callewaert, C.,
Debelius, J., Gonzalez, A., et al. (2018). Best practices for analysing
microbiomes. *Nature Reviews Microbiology*.

</div>

<div id="ref-Lacoste2016">

Lacoste, P., Castro, A., Rendón, B., Pszczólkowski, P., Soto, N.,
Adunka, M. L., Jeffs, J., et al. (2016). Asoleado de cauquenes y
concepción: Apogeo y decadencia de un vino chileno con denominación de
origen. *Idesia*, *34*(1), 85–99. Universidad de Tarapaca.

</div>

<div id="ref-Liu2019">

Liu, P. T., Duan, C. Q., & Yan, G. L. (2019). Comparing the effects of
different unsaturated fatty acids on fermentation performance of
saccharomyces cerevisiae and aroma compounds during red wine
fermentation. *Molecules*, *24*(3). MDPI AG.

</div>

<div id="ref-Liu2018">

Liu, P. T., Yu, K. J., Li, Y. T., Duan, C. Q., & Yan, G. L. (2018). The
content of linoleic acid in grape must influences the aromatic effect of
branched-chain amino acids addition on red wine. *Food Research
International*, *114*, 214–222. Elsevier Ltd.

</div>

<div id="ref-Lonvaud-Funel1999">

Lonvaud-Funel, A. (1999). Lactic acid bacteria in the quality
improvement and depreciation of wine. In *Antonie van leeuwenhoek,
international journal of general and molecular microbiology* (Vol. 76,
pp. 317–331). Springer.

</div>

<div id="ref-Lytra2020">

Lytra, G., Miot-Sertier, C., Moine, V., Coulon, J., & Barbe, J. C.
(2020). Influence of must yeast-assimilable nitrogen content on fruity
aroma variation during malolactic fermentation in red wine. *Food
Research International*, *135*. Elsevier Ltd.

</div>

<div id="ref-Martin2016">

Martin, V., Giorello, F., Fariña, L., Minteguiaga, M., Salzman, V.,
Boido, E., Aguilar, P. S., et al. (2016). De novo synthesis of benzenoid
compounds by the yeast hanseniaspora vineae increases the flavor
diversity of wines. *Journal of Agricultural and Food Chemistry*,
*64*(22), 4574–4583. American Chemical Society.

</div>

<div id="ref-Ozen2015">

Ozen, M., & Dinleyici, E. C. (2015, January). The history of probiotics:
The untold story. Wageningen Academic Publishers. Retrieved from
<https://www.wageningenacademic.com/doi/abs/10.3920/BM2014.0103>

</div>

<div id="ref-Parker2018">

Parker, M., Capone, D. L., Francis, I. L., & Herderich, M. J. (2018).
Aroma precursors in grapes and wine: Flavor release during wine
production and consumption. *Journal of Agricultural and Food
Chemistry*, *66*(10), 2281–2286. American Chemical Society.

</div>

<div id="ref-Quast2013">

Quast, C., Pruesse, E., Yilmaz, P., Gerken, J., Schweer, T., Yarza, P.,
Peplies, J., et al. (2013). The silva ribosomal rna gene database
project: Improved data processing and web-based tools. *Nucleic Acids
Research*, *41*(D1), D590–D596. Oxford Academic.

</div>

<div id="ref-Reguant2003">

Reguant, C., & Bordons, A. (2003). Typification of oenococcus oeni
strains by multiplex rapd-pcr and study of population dynamics during
malolactic fermentation. *Journal of Applied Microbiology*, *95*(2),
344–353. John Wiley & Sons, Ltd.

</div>

<div id="ref-Segata2011">

Segata, N., Izard, J., Waldron, L., Gevers, D., Miropolsky, L., Garrett,
W. S., & Huttenhower, C. (2011). Metagenomic biomarker discovery and
explanation. *Genome Biology*, *12*(6). Genome Biol.

</div>

<div id="ref-Siren2019">

Sirén, K., Mak, S. S. T., Fischer, U., Hansen, L. H., & Gilbert, M. T.
P. (2019). Multi-omics and potential applications in wine production.
*Current Opinion in Biotechnology*, *56*, 172–178.

</div>

<div id="ref-Varela2017">

Varela, C., & Borneman, A. R. (2017). Yeasts found in vineyards and
wineries. *Yeast*, *34*(3), 111–128. John Wiley; Sons Ltd.

</div>

<div id="ref-Yilmaz2014">

Yilmaz, P., Parfrey, L. W., Yarza, P., Gerken, J., Pruesse, E., Quast,
C., Schweer, T., et al. (2014). The silva and "all-species living tree
project (ltp)" taxonomic frameworks. *Nucleic Acids Research*, *42*(D1),
D643–D648. Oxford Academic.

</div>

</div>
