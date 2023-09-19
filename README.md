DDIT4L monocyte extraction validation
<p> Last update: 2023-09-19

* Flow analysis was performed using R (4.3.1 -- "Beagle Scouts") in RStudio ('2023.6.1.524' -- "Mountain Hydrangea") using mainly `ggcyto` and `flowCore` (see 'R session info' below). 
** The .rmd file in this folder was used to generate the analysis.

==================================================================

Purpose: to obtain viable monocytes via positive selection (CD14+) to validate the RNA expression of DDIT4L in term monocytes (controls: adult)

==================================================================
![Figure 1 - Flow gating strategy and samples](https://github.com/liamg15/Flow_cytometry/blob/main/Final%20figures/flow_layout_example_final.tif?raw=true)
Experimental set-up:

* For RT-PCR:
- 4 term samples (TS220, TS549, TS555, TS579)
- 3 adult samples (FH00039, FH00040, VCW135-1-14)

* For purification validation and staining
- 1 CD14 depleted CBMC sample (TS218)
- 1 unprocessed term CBMC (TS519)
- 1 unstained, unprocessed term CBMC (TS519)

* Flow panel
- FVD eF780
- CD14 BV421
- CD3 and CD19 FITC

==================================================================

Folder breakdown:

1) FCS files - contains all .FCS files from the positive selection, including an unstained control, unprocessed CBMC, and CD14 depleted CBMC.
2) Final figures - contains final figures after flow analysis of cell populations in .tiff format (600dpi)
3) Gating strategy - .pdf files and .ai files used to generate final figures plus additional figures from flow analysis
4) Protocol - contains CBMC/PBMC thawing and CD14 positive and negative selection protocols
5) .old - old files not relevant to final analysis but generated during development of this folder

==================================================================

R session info:
attached base packages:
[1] stats     graphics  grDevices utils     datasets  methods   base     

other attached packages:
 [1] here_1.0.1           lubridate_1.9.2      forcats_1.0.0        stringr_1.5.0        dplyr_1.1.3         
 [6] purrr_1.0.2          readr_2.1.4          tidyr_1.3.0          tibble_3.2.1         tidyverse_2.0.0     
[11] ggcyto_1.28.1        flowWorkspace_4.12.2 ncdfFlow_2.46.0      BH_1.81.0-1          flowCore_2.12.2     
[16] ggplot2_3.4.3       

loaded via a namespace (and not attached):
 [1] utf8_1.2.3          generics_0.1.3      stringi_1.7.12      lattice_0.21-8      hms_1.1.3          
 [6] digest_0.6.33       magrittr_2.0.3      timechange_0.2.0    evaluate_0.21       grid_4.3.1         
[11] RColorBrewer_1.1-3  fastmap_1.1.1       rprojroot_2.0.3     plyr_1.8.8          graph_1.78.0       
[16] gridExtra_2.3       fansi_1.0.4         scales_1.2.1        XML_3.99-0.14       Rgraphviz_2.44.0   
[21] cli_3.6.1           rlang_1.1.1         RProtoBufLib_2.12.1 Biobase_2.60.0      munsell_0.5.0      
[26] withr_2.5.0         yaml_2.3.7          cytolib_2.12.1      tools_4.3.1         tzdb_0.4.0         
[31] colorspace_2.1-0    BiocGenerics_0.46.0 vctrs_0.6.3         R6_2.5.1            matrixStats_1.0.0  
[36] stats4_4.3.1        lifecycle_1.0.3     zlibbioc_1.46.0     S4Vectors_0.38.1    pkgconfig_2.0.3    
[41] pillar_1.9.0        hexbin_1.28.3       gtable_0.3.4        data.table_1.14.8   glue_1.6.2         
[46] Rcpp_1.0.11         xfun_0.40           tidyselect_1.2.0    rstudioapi_0.15.0   knitr_1.44         
[51] htmltools_0.5.6     rmarkdown_2.24      compiler_4.3.1
