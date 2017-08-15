# SPurS Project: Identifying Shifts in Purifying Selection
Sites in the genome under strong [purifying selection](https://www.nature.com/scitable/topicpage/negative-selection-1136) are highly conserved (invariant) across species, regardless of their phylogenetic relationship. In contrast, SPurS sites exhibit conservation among species belonging to the same group or taxonomic clade, and variation between species in different groups or clades.

For example, a site with one amino acid in mammals and a different amino acid in birds represent a likely *shift* from one residue to another between the two species groups, which has been conserved under purifying selection over time.

<p align="center">
  <img src="https://user-images.githubusercontent.com/6342355/29278014-c89e3266-8113-11e7-8da3-c8412a20359b.jpg" border="5"/>
</p>

The SPurS program calculates a Psi-value (Fig.1) for each site in a protein alignment, and the results can be visualized in SPurS plots (Fig.2, below) by using the [Genomic Hyperbrowser SPurS tool](https://hyperbrowser.uio.no/spurs). When compared to a matched simulated dataset, these results can be compared to determine whether proteins are enriched for SPurS sites. These sites are likely involved in speciation, or divergence between species, and are thus highly informative for evolutionary genomics.

<p align="center">
  <img src="https://user-images.githubusercontent.com/6342355/29311905-974b711a-81b3-11e7-8e30-79c53a810b6c.jpg" "width=800"/>
</p>

Fig.5 (above) shows SPurS plots for multiple-sequence alignments of FAM81A and SLC1A3 across 76 species, with Psi-values calculated between mammals and birds.

Without any statistical analyses, an eyeball assessment of these two SPurS plots (simulated vs. real data) reveals a notable difference in the proportion of sites exhibiting high Psi-values for FAM81A, but not for SLC1A3. These observations are confirmed by a Pearson’s Chi-squre test, which reveals a statistically significant difference between the proportion of SPurS sites (where Psi = 1) in FAM81A (p-value = 0.0001) and not for SLCA13 (p-value = 0.84).

The interpretation of these findings is that FAM81A is enriched for SPurS sites, relative to the null, while SLCA13 is not. This means that FAM81A may be involved in physiological or functional differences between birds and mammals, and should be followed up as a potential mechanism of speciation.
