---
layout: default
title: 1BIF
author: Jordi Villà-Freixa
permalink: /1bif/

---
 <head>
    <meta charset="utf-8">
    <title>{{ page.title }}</title>
<script src="https://cdn.jsdelivr.net/npm/babel-polyfill/dist/polyfill.min.js"></script>
    <!-- Web component polyfill (only loads what it needs) -->
<script src="https://cdn.jsdelivr.net/npm/@webcomponents/webcomponentsjs/webcomponents-lite.js" charset="utf-8"></script>
    <!-- Required to polyfill modern browsers as code is ES5 for IE... -->
<script src="https://cdn.jsdelivr.net/npm/@webcomponents/webcomponentsjs/custom-elements-es5-adapter.js" charset="utf-8"></script>

<link rel="stylesheet" type="text/css" href="https://www.ebi.ac.uk/pdbe/pdb-component-library/css/pdbe-molstar-1.2.1.css">
<script type="text/javascript" src="https://www.ebi.ac.uk/pdbe/pdb-component-library/js/pdbe-molstar-component-1.2.1.js"></script>
<style>
        #myViewer{
          float:none;
          width:400px;
          height:400px;
          position:relative;
        }
    </style>
  </head>

<h1> Anàlisi de les relacions seqüència-estructura-funció de la proteïna bifuncional fosfoquinasa/fructosa 2,6-bifosfatasa (PDB: 1BF1)</h1>

- [Estructura secundària](#estructura-secundària)
- [Estructura supersecundària](#estructura-supersecundària)
- [Plegament](#plegament)
- [Funció](#funció)


 El codi [PDB:1BF1](https://www.rcsb.org/structure/1bf1) correspon a l'estructura de l'enzim bifuncional 6-fosfofructo-2-quinasa/fructosa-2,6-bifosfatasa, que catalitza tant la síntesi com la degradació de la frustosa-2,6-bifosfat, un metabòlit clau en el metabolisme de la glucosa. El codi [UNIPROT:P25114](https://www.uniprot.org/uniprot/P25114), amb una gran conservació de seqüència.


La seqüència de la proteïna al PDB és

```fasta
>1BIF_1|Chain A|6-PHOSPHOFRUCTO-2-KINASE/ FRUCTOSE-2,6-BISPHOSPHATASE|Rattus norvegicus (10116)
MASPRELTQNPLKKIFMPYSNGRPALHASQRGVCMTNCPTLIVMVGLPARGKTYISKKLTRYLNFIGVPTREFNVGQY
RRDMVKTYKSFEFFLPDNEEGLKIRKQCALAALNDVRKFLSEEGGHVAVFDATNTTRERRAMIFNFGEQNGYKTFFVE
SICVDPEVIAANIVQVKLGSPDYVNRDSDEATEDFMRRIECYENSYESLDEEQDRDLSYIKIMDVGQSYVVNRVADHI
QSRIVYYLMNIHVTPRSIYLCRHGESELNLKGRIGGDPGLSPRGREFSKHLAQFISDQNIKDLKVFTSQMKRTIQTAE
ALSVPYEQFKVLNEIDAGVCEEMTYEEIQDHYPLEFALRDQDKYRYRYPKGESYEDLVQRLEPVIMELERQENVLVIC
HQAVMRCLLAYFLDKAAEELPYLKCPLHTVLKLTPVAYGCKVESIFLNVAAVNTHRDRPQNVDISRPSEEALVTVPAH
Q
```

Pots visualitzar la proteïna en aquesta finestra proveïda per [Mol*](https://molstar.org):

<p>
<div id="myViewer">
<pdbe-molstar id="pdbeMolstarComponent" molecule-id="1bif" hide-controls="true"></pdbe-molstar>
</div>
</p>
<br>  

## Estructura secundària

L'estructura presenta tant hèlix alfa com fulles beta

|![](../figures/1bif_2nd.png)|
|:--:|
|Imatge de la proteïna mostrant els elements d'estructura secundària.|

La següent figura mostra la seqüència de la proteïna i les regions amb hèlix alfa (groc) i fulles beta (verd)

|![](../figures/1bif_seq.png)|
|:--:|
|Seqüència de la proteïna mostrant els elements d'estructura secundària|

El fitxer PDB conté informació sobre l'estructura secundària. Anem a [visualitzar la proteïna a Chimera](../code/1bif.py). 

```
HELIX    1   1 LYS A   51  PHE A   64  1                                  14    
HELIX    2   2 VAL A   74  VAL A   82  1                                   9    
HELIX    3   3 PHE A   88  PHE A   91  5                                   4    
HELIX    4   4 GLU A   96  SER A  118  1                                  23    
HELIX    5   5 ARG A  134  ASN A  147  1                                  14    
HELIX    6   6 PRO A  161  VAL A  171  1                                  11    
HELIX    7   7 SER A  183  GLU A  198  1                                  16    
HELIX    8   8 HIS A  232  ASN A  243  1                                  12    
HELIX    9   9 GLU A  260  LYS A  264  1                                   5    
HELIX   10  10 PRO A  275  GLN A  291  1                                  17    
HELIX   11  11 LYS A  304  ALA A  312  1                                   9    
HELIX   12  12 LYS A  321  LEU A  323  5                                   3    
HELIX   13  13 GLY A  329  CYS A  331  5                                   3    
HELIX   14  14 TYR A  336  HIS A  342  1                                   7    
HELIX   15  15 PRO A  344  GLN A  352  1                                   9    
HELIX   16  16 TYR A  365  ARG A  381  1                                  17    
HELIX   17  17 GLN A  391  PHE A  401  1                                  11    
HELIX   18  18 ALA A  406  TYR A  411  1                                   6    
HELIX   19  19 SER A  457  ALA A  460  1                                   4    
SHEET    1   A 6 SER A 223  ASN A 227  0                                        
SHEET    2   A 6 TYR A 214  MET A 218 -1  N  MET A 218   O  SER A 223           
SHEET    3   A 6 LYS A 150  SER A 156  1  N  PHE A 153   O  ILE A 215           
SHEET    4   A 6 THR A  39  VAL A  44  1  N  LEU A  40   O  LYS A 150           
SHEET    5   A 6 VAL A 124  ASP A 128  1  N  ALA A 125   O  THR A  39           
SHEET    6   A 6 THR A  69  ASN A  73  1  N  ARG A  70   O  VAL A 124           
SHEET    1   B 5 CYS A 429  PHE A 435  0                                        
SHEET    2   B 5 THR A 418  PRO A 424 -1  N  THR A 423   O  LYS A 430           
SHEET    3   B 5 ILE A 251  ARG A 255 -1  N  LEU A 253   O  LEU A 420           
SHEET    4   B 5 VAL A 385  CYS A 389  1  N  VAL A 385   O  TYR A 252           
SHEET    5   B 5 LYS A 297  THR A 300  1  N  LYS A 297   O  LEU A 386           
```

Notar la presència d'alfa hèlix (etiquetades amb un "1") i també d'hèlix 3-10 (etiquetades amb un "5").

## Estructura supersecundària

La figura mostra l'estructura amb un codi de colors progressiu que permet identificar la regió N-terminal (blau) i la regió C-terminal (vermell).

|![](../figures/1bif_rainbow.png)|
|:--:|
|Imatge de la proteïna amb la representació amb colors de fred (blau) a calent (vermell) en funció de la seqüència.|

Podem observar diversos motius d'estructura supersecundària, que es poden deduir també de l'observació de la seqüència a la figura de més amunt.

El monomer de la proteïna està clarament dividit en dos dominis funcionals, que veurem més avall com estan involucrats en la seva funció. Per ara, notem que el domini N-terminal (tons blaus a la figura de més amunt) correspon al domini fosfofructoquinasa (hi podem identificar també la molècula [ATP$\gamma$S](https://pubchem.ncbi.nlm.nih.gov/compound/44123300), en el fitxer PDB identificada com a AGS, que es col·loca al mateix lloc on enllaçaria la molèculña d'ATP del domini quinasa).

| motiu | regio | imatge |
|:-------:|:-------:|:--------:|
|   $\beta$-hairpin    | per ex.  ```HTVLKLTPVAYGCKVESIF```    |   ![](../figures/1bif_hairpin.png)     |
|    P-loop / Walker motif  |    ```GLPARGKT```   |    ![](../figures/1bif_ploop.png)       |
|     $\beta-\alpha$    |   per ex.  ```TLIVMVGLPARGKTYISKKLTRYLNFIG``` |    ![](../figures/1bif_betaalfa.png)       |

## Plegament

Es tracta d'una proteïna $\alpha/\beta$, amb dos dominis i plegaments clarament diferenciats

 1. plegament de tipus *P-loop kinase* [segons la clasificació a SCOP](https://scop.mrc-lmb.cam.ac.uk/term/8019198) en el domini N-terminal;
 1. plegament de tipus *Phosphoglycerate mutase* [segons la clasificació a SCOP](https://scop.mrc-lmb.cam.ac.uk/term/8019202) en el domini C-terminal.

|![](../figures/1BIF_SCOP1.png)![](../figures/1BIF_SCOP1.png)|
|:--:|
|Estructura jeràrquica dels dos dominis presents a PDB:1BIF|

Aquests dominis s'identifiquen com a par de les superfamílies *P-loop containing nucleotide triosephosphate hydrolases* i *Phosphoglycerate mutase-like* [segons CATH](http://www.cathdb.info/search?q=1bif).

## Funció

Podem començar per [cercar a PFAM el codi uniprot de la proteïna](http://pfam.xfam.org/protein/P01112). Veiem que es tracta d'una proteïna amb dos dominis ben caracteritzats:

|![](../figures/1bif_pfam1.png)|
|:--:|
|Taula resum dels dominis PFAM per al PDB:1BIF, UNIPROT: P25114|

Podem aleshores explorar l'entrada per a cadascun d'aquests dominis: 

 1. PFAM: PF01591/6PF2K, quinasa que enllaça dos substrats: ATP i beta-D-fructosa 6-fosfat. El domini es troba en més de [100 arquitectures diferents](http://pfam.xfam.org/family/6PF2K#tabview=tab1), i vora [1500 espècies](http://pfam.xfam.org/family/6PF2K#tabview=tab7), majoritàriament eucariotes.
 2. PFAM: PF00300/His_Phos_1, fosfatases d'histidina. El domini es troba en més de [500 arquitectures diferents](http://pfam.xfam.org/family/His_Phos_1#tabview=tab1), i més de [8000 espècies](http://pfam.xfam.org/family/His_Phos_1#tabview=tab7), de taxons molt diversos.

L'estudi dels logos HMM dels dos dominis, mostra informació sobre els seus centres actius:

1. (http://pfam.xfam.org/family/PF01591#tabview=tab4) ens mostra una regió molt enriquida en glicines corresponent al P-loop, i també la gran conservació de la Treonina 52 del fitxer PDB (posició 27 en el logo HMM), que és essencial per a la coordinació de l'ió magnesi, que participa en la reacció d'hidròlisi de l'ATP, com es pot apreciar en el centre actiu de la proteïna:

|![](../figures/1bif_ploop.png)|
|:--:|
|regió d'enllaç als fosfats de l'ATP  en el domini N-terminal de la proteïna PDB:1BIF.|

2. (http://pfam.xfam.org/family/PF00300#tabview=tab4) ens mostra una gran conservació de residus polars i carregats, en especial dues histidines (veure la figura 5 de l'[article](https://www.cell.com/structure/fulltext/S0969-2126(96)00109-8) on es publicava l'estructura 1BIF)

|![](../figures/1bif_centreactiu2.png)|
|:--:|
|centre actiu on es produeix la hidròlisi de la fructosa-2,6-bifosfatasa en el domini C-terminal de la proteïna PDB:1BIF.|

Altres residus altament conservats que s'aprecien al logo PFAM tenen tasques importants en l'activitat de la proteïna.
