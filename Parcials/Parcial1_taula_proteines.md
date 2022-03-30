---
layout: default
title: Exemples d'estudi d'estructures de proteïnes
permalink: /estructura/
---


- [Exemples d'anàlisi d'estructures](#exemples-danàlisi-destructures)
  - [PDB: 5P21](#pdb-5p21)
    - [Estructura secundària](#estructura-secundària)
    - [Estructura supersecundària](#estructura-supersecundària)
    - [Plegament](#plegament)
    - [Funció](#funció)
  - [PDB: 1PRN](#pdb-1prn)
    - [Estructura secundària](#estructura-secundària-1)
    - [Estructura supersecundària](#estructura-supersecundària-1)
    - [Plegament](#plegament-1)
    - [Funció](#funció-1)
  - [PDB: 1BL8](#pdb-1bl8)
    - [Estructura secundària](#estructura-secundària-2)
    - [Estructura supersecundària](#estructura-supersecundària-2)
    - [Plegament](#plegament-2)
    - [Funció](#funció-2)
  - [PDB: 2RH1](#pdb-2rh1)
    - [Estructura secundària](#estructura-secundària-3)
    - [Estructura supersecundària](#estructura-supersecundària-3)
    - [Plegament](#plegament-3)
    - [Funció](#funció-3)
  - [PDB: 1BIF](#pdb-1bif)
    - [Estructura secundària](#estructura-secundària-4)
    - [Estructura supersecundària](#estructura-supersecundària-4)
    - [Plegament](#plegament-4)
    - [Funció](#funció-4)
  - [PDB: 3H8Q](#pdb-3h8q)
    - [Estructura secundària](#estructura-secundària-5)
    - [Estructura supersecundària](#estructura-supersecundària-5)
    - [Plegament](#plegament-5)
    - [Funció](#funció-5)


# Exemples d'anàlisi d'estructures
 
## PDB: 5P21

 El codi [PDB:5P21](https://www.rcsb.org/structure/5p21) correspon a l'estructura de la proteïna H-RAS p21,codi [UNIPROT:P01112](https://www.uniprot.org/uniprot/P01112), amb una gran conservació de seqüència pel que es pot veure a l'[alineament](https://www.rcsb.org/uniprot/P01112) que el propi PDB ens dona.



La seqüència de la proteïna al PDB és

```fasta
>5P21
MTEYKLVVVGAGGVGKSALTIQLIQNHFVDEYDPTIEDSYRKQVVIDGETCLLDILDTAGQEEYSAMRDQYMRTGEGFLCVFAINNTKSFEDIHQYREQIKRVKDSDDVPMVLVGNKCDLAARTVESRQAQDLARSYGIPYIETSAKTRQGVEDAFYTLVREIRQH
```

### Estructura secundària 

L'estructura presenta tant hèlix alfa com fulles beta

![imatge de la proteïna mostrant els elements d'estructura secundària](../figures/5p21_2nd.png)

La següent figura mostra la seqüència de la proteïna i les regions amb hèlix alfa (groc) i fulles beta (verd)

![Seqüència de la proteïna mostrant els elements d'estructura secundària](../figures/5p21_seq.png)

### Estructura supersecundària 

La figura mostra l'estructura amb un codi de colors progressiu que permet identificar la regió N-terminal (blau) i la regió C-terminal (vermell). 

![Imatge de la proteïna amb la representació amb colors de fred (blau) a calent (vermell) en funció de la seqüència](../figures/5p21_rainbow.png)

Malauradament el fitxer PBD no conté massa informació sbre l'estructura secundària i no en podem treure massa profit, en aquest cas. Anem a [visualitzar la proteïna a Chimera](../code/5p21.py). Podem observar diversos motius d'estructura supersecundària, que es poden deduir també de l'observació de la seqüència a la figura de més amunt.

| motiu | regio | imatge |
|:-------:|:-------:|:--------:|
|   $\beta$-hairpin    |   ```EDSYRKQVVIDGETCLLDILDT```    |   ![](../figures/5p21_hairpin.png)     |
|    P-loop   |    ```MTEYKLVVVGAGGVGKSALTIQLIQN```   |    ![](../figures/5p21_ploop.png)       |
|     motius $\beta-\alpha-\beta$ amb la fulla $\beta$ tancada    |    ```SAMRDQYMRTGEGFLCVFAINNTKSFED```<br>```IHQYREQIKRVKDSDDVPMVLVGNKCDL```<br>```AARTVESRQAQDLARSYGIPYIETSAKT```<br>```RQGVEDAFYTLVREIR``` |    ![](../figures/5p21_betaalphabeta.png)       |

### Plegament 

Es tracta d'una proteïna $\alpha/\beta$, amb un plegament de tipus *G-domain-like* quin representant és PDB:1CTQ [segons la clasificació a SCOP](https://scop.mrc-lmb.cam.ac.uk/term/8019404) 

![Estructura jeràrquica del domini al qual pertany PDB:5P21, representada a SCOP per PDB:1CTQ](../figures/1CTQ_SCOP.png)

i de domini que forma part de la superfamília *P-loop containing nucleotide triosephosphate hydrolases* [segons CATH](http://www.cathdb.info/search?q=5p21).

### Funció

Podem començar per [cercar a PFAM el codi uniprot de la proteïna](http://pfam.xfam.org/protein/P01112). Veiem que es tracta d'una proteïna amb un sol domini ben caracteritzat: 

![Taula resum dels dominis PFAM per al PDB:5p21, UNIPROT: P01112](../figures/5p21_pfam1.png). 

Podem aleshores explorar l'entrada per a aquest domini específic: PFAM: PF00071, i observem que es tracta d'una GTPasa. El domini concret Ras està altament distribuït, trobat en més de [1500 arquitectures diferents](http://pfam.xfam.org/family/PF00071#tabview=tab1), vora [2000 espècies](http://pfam.xfam.org/family/PF00071#tabview=tab7)

/* set css rules for styling the logo */
<link rel="stylesheet" type="text/css" href="hmm_logo.min.css">

/* make sure jQuery has been loaded */
<script src="jquery-1.8.2.min.js"></script>

/* load in the hmm_logo code */
<script src="hmm_logo.min.js"></script>

/* At the location where you want the logo to appear in your page */
<div id="logo" class="logo" data-logo="ras.json"></div>

/* finally run the call to render the logo on page load */
<script>
  $(document).ready(function () {
    $('#logo').hmm_logo();
  });
</script>

## PDB: 1PRN


### Estructura secundària 
### Estructura supersecundària 
### Plegament 
### Funció


## PDB: 1BL8



### Estructura secundària 
### Estructura supersecundària 
### Plegament 
### Funció


## PDB: 2RH1



### Estructura secundària 
### Estructura supersecundària 
### Plegament 
### Funció

## PDB: 1BIF


### Estructura secundària 
### Estructura supersecundària 
### Plegament 
### Funció

## PDB: 3H8Q


### Estructura secundària 
### Estructura supersecundària 
### Plegament 
### Funció
