---
layout: default
title: Pràctica de Relacions seqüència-estrcutura-funció
permalink: /practica2/
---

# Activitat S2: Relacions seqüència-estructura-funció

(Química i Enginyeria de Proteïnes, 2021-2022)

## Preparació

1. Instal·lació de [Jalview](http://www.jalview.org/getdown/release/#)
2. Familiarització amb **[Pfam](https://pfam.xfam.org/)**
3. [Tutorial](./TutorialPFAM.pdf) de PFAM

## EXERCICI 1) Exemple d'ús de PFAM

### Qüestió

Considereu la següent proteina. Fent servir informació dels dominis presents indiqueu de quin tipus de proteïna es tracta. Raoneu la vostra resposta: Indiqueu quins dominis presenta, a quines posicions, quines funcions porten associades, a quin clan PFAM, etc. Il·lustreu la vostra resposta amb alineaments trobats a PFAM, amb estructures del PDB, etc.

```
>protein x
MAEDDPYLGRPEQMFHLDPSLTHTIFNPEVFQPQMALPTDGPYLQILEQPKQRGFRFRYV
CEGPSHGGLPGASSEKNKKSYPQVKICNYVGPAKVIVQLVTNGKNIHLHAHSLVGKHCED
GICTVTAGPKDMVVGFANLGILHVTKKKVFETLEARMTEACIRGYNPGLLVHPDLAYLQA
EGGGDRQLGDREKELIRQAALQQTKEMDLSVVRLMFTAFLPDSTGSFTRRLEPVVSDAIY
DSKAPNASNLKIVRMDRTAGCVTGGEEIYLLCDKVQKDDIQIRFYEEEENGGVWEGFGDF
SPTDVHRQFAIVFKTPKYKDINITKPASVFVQLRRKSDLETSEPKPFLYYPEIKDKEEVQ
RKRQKLMPNFSDSFGGGSGAGAGGGGMFGSGGGGGGTGSTGPGYSFPHYGFPTYGGITFH
PGTTKSNAGMKHGTMDTESKKDPEGCDKSDDKNTVNLFGKVIETTEQDQEPSEATVGNGE
VTLTYATGTKEESAGVQDNLFLEKAMQLAKRHANALFDYAVTGDVKMLLAVQRHLTAVQD
ENGDSVLHLAIIHLHSQLVRDLLEVTSGLISDDIINMRNDLYQTPLHLAVITKQEDVVED
LLRAGADLSLLDRLGNSVLHLAAKEGHDKVLSILLKHKKAALLLDHPNGDGLNAIHLAMM
SNSLPCLLLLVAAGADVNAQEQKSGRTALHLAVEHDNISLAGCLLLEGDAHVDSTTYDGT
TPLHIAAGRGSTRLAALLKAAGADPLVENFEPLYDLDDSWENAGEDEGVVPGTTPLDMAT
SWQVFDILNGKPYEPEFTSDDLLAQGDMKQLAEDVKLQLYKLLEIPDPDKNWATLAQKLG
LGILNNAFRLSPAPSKTLMDNYEVSGGTVRELVEALRQMGYTEAIEVIQAASSPVKTTSQ
AHSLPLSPASTRQQIDELRDSDSVCDSGVETSFRKLSFTESLTSGASLLTLNKMPHDYGQ
EGPLEGKI
```

NOTA: A part del `sequence search` link a la web de PFAM també pots utilitzar el servidor [HMMER](https://www.ebi.ac.uk/Tools/hmmer/search/hmmscan) de l'EBI, més ràpid. Selecciona la base de dades PFAM per fer la cerca).

### Resposta

Usant la web de l'EBI, i fent una cerca de la seqüència, obtenim la imatge següent:

![](figures/Pr2Ex1a.png)

La taula mostra 4 clars dominis:

* [Rel homology DNA-binding domain](http://pfam.xfam.org/family/RHD_DNA_bind) 	
* [Rel homology dimerisation domain](http://pfam.xfam.org/family/RHD_dimer) 	
* Ankyrin repeats (diverses còpies i variants: [ANK](http://pfam.xfam.org/family/Ank), [ANK_2](http://pfam.xfam.org/family/Ank_2) i [ANK_4](http://pfam.xfam.org/family/Ank_4)) 	
* [Death domain](http://pfam.xfam.org/family/Death)

Com expliquem al [Tutorial](./TutorialPFAM.pdf) de PFAM, observem famílies PFAM (dominis RHD_DNA_bind,  RHD_dimer i DEATH), així com dominis repetits (Ankyrin, en aquest cas).

La informació a les pàgines de PFAM ens mostra que:  

* el domini RHD_DNA_bind és típic de factors de transcripció, entre els quals la proteïna NF-KB;
* el domini RHD_Dimer ajuda a la dimerització del domini RHD_DNA_bind, que té sempre en N-terminal;
* el domini DEATH està composat de 6 hèlix alfa;
* finalment, els repeats Ankyrin
  

Podem usar Jalview per visualitzar l'alineament en que es basa cadascun dels dominis.

Una cerca amb BLAST a NCBI ens mostra que, certament,  es tracta de la proteïna NF-KB, i entrant amb més detall als resultats del BLAST obtenim informació sobre els dominis des del propi NCBI.

![](figures/Pr2Ex1b.png)

## EXERCICI 2) Exemple d'ús de PFAM

Considereu les proteïnes amb codis UNIPROT: P00749, P00734, P00750 i P00747. Quins tipus de dominis presenten aquestes proteïnes? Presenten algun tipus de dominis comuns? Podeu especular quelcom sobre la seva relació funcional basant-vos en la composició de dominis i la seva conservació? PISTA: Formen part de la [cascada de coagulació](https://www.osmosis.org/answers/coagulation-cascade).

## EXERCICI 3) Exemple d'ús de PFAM

Considereu aquestes 3 proteïnes (codi Uniprot entre parèntesis): 

* Lin-49 (Q20318) de C. Elegans
* Peregrin (P55201) de H. Sapiens
* YOR031W (Q12311) de S. cerevisiae

Primer, definiu quin podria ser l'ancestre comú d'aquestes tres proteïnes, tenint en compte la seva composició de dominis. Justifiqueu la vostra resposta. Un cop definit l'ancestre comú, hipotetitzeu sobre el possible camí evolutiu d’aquestes tres proteïnes. Justifiqueu la vostra resposta.