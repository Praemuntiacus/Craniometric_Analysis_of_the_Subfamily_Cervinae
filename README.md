# Craniometric_Analysis_of_the_Subfamily_Cervinae
Supplimentary materials to the article "A Craniometric Analysis of the Subfamily Cervinae (Cervidae, Mammalia)"

***
**THE AIM OF THE STUDY**
The objective of this study is to conduct a Principal Component Analysis (PCA) on cranial measurements of both fossil and modern deer belonging to the subfamily Cervinae, with the goal of characterizing the cranial morphological diversity within this taxonomic group. The repository includes the dataset (available in both [Excel](https://github.com/Praemuntiacus/Craniometric_Analysis_of_the_Subfamily_Cervinae/blob/main/Table%201S.%20CERVIDAE%20CRANIAL%20MEASUREMENTS.xlsx) and [CSV](https://github.com/Praemuntiacus/Craniometric_Analysis_of_the_Subfamily_Cervinae/blob/main/Table%201S.%20CERVIDAE%20CRANIAL%20MEASUREMENTS.csv) formats) and a [Jupyter Notebook](https://github.com/Praemuntiacus/Craniometric_Analysis_of_the_Subfamily_Cervinae/blob/main/CERVIDAE_CRANIOMETRY.ipynb) showcasing all stages of data preprocessing, imputation, analysis, and diagram generation.

***
**RESEARCH METHODS**

The craniological material comprises over 300 skulls of both modern and fossil representatives of the subfamily Cervinae. The fossil and modern osteological specimens utilized in this study are curated at various institutions, including the Institute of Zoology of the State University of Moldova (IZM), Republic of Moldova; the Institute of Zoology of the University of Wroclaw (IZW), Poland; the Museum of Geology and Paleontology of the University of Florence (MGUF), Italy; the Muséum national d'Histoire naturelle (MNHN), Paris, France; the Museum of Paleontology of the Department of Earth Sciences (MPS), University of Rome “Sapienza”, Italy; the Natural History Museum “Grigore Antipa” (NHMB), Bucharest, Romania; the Natural History Museum of London (NHML), United Kingdom; the Natural History Museum “La Specola” (NHMF), University of Florence, Italy; the Paleontological Museum of the University “Claude Bernard” Lyon 1 (PMUL), France; and the State Museum of Natural History of Stuttgart (SMNH), Germany.
Some cranial measurements of *Cervus elaphus* are adapted from Heptner and Tzalkin (1947), the data on *Cervus elaphus siciliae* are adapted from Gliozzi et al. (1993), the data on *Praedama giulii* are adapted from Breda et al. (2020), while cranial measurements for *Candiacervus ropalophorus* are adapted from Schilling and Roessner (2021). Detailed information regarding cranial specimens, their collection numbers, institutions of curation, and measurements can be found in Table 1S of the supplementary materials.

The following cranial measurements were obtained:

<p align="center">
  <i>Scheme of cranial measurements</i>
</p>

<img src="https://github.com/Praemuntiacus/Craniometric_Analysis_of_the_Subfamily_Cervinae/blob/main/figure-1.jpg" alt="image" width="500" style="display: block; margin: 0 auto;">



1 •	Condylobasal length of the skull (CBL): Measured from the prosthion point to the posterior edges of the occipital condyles;

1a •	Condylodental length of the skull (L_P2_occiput): Measured from the anterior edge of the P2 alveolus to the posterior edges of the occipital condyles;

•	Length of basioccipitale (L_basiocc): Measured from the posterior edge of the oc-cipital condyles to the suture between basioccipital and basisphenoid (*not shown on the scheme*);

2 •	Length of the upper tooth row (L_P2_M3): Measured from the anterior edge of the P2 crown to the posterior edge of the M3 crown;

3 •	Length of the upper molar series (L_M1_M3): Taken as the maximal value from the anterior edge of the M1 crown to the posterior edge of the M3 crown;

4 •	Length of the upper premolar series (L_P2_P4): Taken as the maximal value from the anterior edge of the P2 crown to the posterior edge of the P4 crown;

5 •	Length of the anterior part of the skull before the tooth row (L_P2_prosth): The distance between the anterior edge of the alveolus of P2 and the prosthion point;

6 •	Length of the posterior part of the skull (L_M3_occ_cond): The distance between the anterior edge of the alveolus of M3 and the posterior edge of the occipital con-dyles;

7 •	Length of the braincase (L_bregma_inion): The distance between the bregma point and the inion point;

8 •	Occipital breadth (W_occiput): Measured as the maximum breadth of the occiput;

9 •	Occipital height (H_occiput): Measured from the basicranium to the opis-thocranion;

10 •	Breadth of occipital condyles (W_occ_cond);

11 •	Length of face (L_orbit_prosth): Measured from the anterior edge of the orbits to the prosthion;

12 •	Length of the splanchocranium (L_bregma_prosth): Measured from bregma to the prosthion;

13 •	Skull breadth at M3 (W_at_M3): The measurement taken between the alveolar edges in the middle of the right and left M3;

14 •	Skull breadth at P2 (W_at_P2): The measurement taken between the alveolar edg-es in the middle of the right and left P2;

15 •	Breadth of the muzzle (W_rostrum): Measured behind the upper canines or at the suture between the maxillary and premaxillary bones;

17 •	Breadth above orbits (W_at_orbits): Measured above the orbital centers;

18 •	Frontal breadth (W_frontal; in males only): Measurement taken at the frontal constriction before the pedicles;

•	Breadth of the neurocranium (W_braincase): Measurement taken behind the ped-icles in males and as the maximal breadth of the braincase in females (*not shown on the scheme*);

20 •	Diameter of the orbit (D_orbit; vertical);

21 •	Length of the frontal suture (L_front_sut): From bregma to nasion;

23 •	Length of the nasalia (L_nasal): From nasion to rhinion

Some skulls, particularly fossils, exhibit varying degrees of incompleteness. The majority of specimens analyzed in this study are from male individuals, with female specimens included only when their measurements provided valuable insights mini-mally influenced by sexual dimorphism. Mean values of cranial measurements for species and subspecies (for instance, in the case of red deer Cervus elaphus, which is represented by subspecies with significantly different body sizes) were utilized for analysis. While certain species are represented by only a single specimen or a small sample size, the behavior of data from these cases within the context of the entire da-taset suggests that this limitation has minimal impact on the study's results.

The cranial material comprises over 400 skulls of both modern and fossil representatives of the subfamily Cervinae. The craniometric data for many fossil and modern specimens are incomplete, as illustrated in this diagram (the measurements are groupped by species or servid form as mean):

<p align="center">
  <i>Missing data by species or cervid form</i>
</p>

<img src="https://github.com/Praemuntiacus/Craniometric_Analysis_of_the_Subfamily_Cervinae/blob/main/Fig_1S_missing_data.jpg" alt="image" width="500" style="display: block; margin: 0 auto;">

Linear and multilinear correlations were found to be the most suitable methods for imputing missing data in this study.

 ***
 **BIBLIOGRAPHIC SOURCES**
 
Heptner, V.G.; Zalkin, V.I. Deer of the USSR (Systematics and Zoogeography). Trans. Study Fauna Flora USSR, Moscow Soc. Nat. 1947, 10(25), 1-176 (in Russian).

Breda, M., Lister, A., Kahlke, R.D., 2020. New results on cervids from the Early Pleistocene site of Untermassfeld. In: Kahlke, R.D. (Ed.), The Pleistocene of Untermassfeld near Meiningen (Thüringen, Germany), Part 4. Monographien des Rö-misch-Germanisches Zentralmuseum, 40 (4): 1197-1249, Mainz: Verlag des Römisch-Germanischen Zentralmuseums.

Gliozzi, E.; Malatesta, A.; Scalone, E. Revision of Cervus elaphus siciliae Pohlig, 1893, Late Pleistocene endemic seer of the Siculo-Maltese District. Geol. Rom. 1993, 29, 307-353.

Schilling, A.M.; Roessner, G.E. New skull material of Pleistocene dwarf deer from Crete (Greece). CR Palevol 2021, 20(9), 141-164.

