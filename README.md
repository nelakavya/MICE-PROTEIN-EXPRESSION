# MICE-PROTEIN-EXPRESSION
MICE PROTEIN EXPRESSION


Abstract
Down syndrome (DS) is a chromosomal disorder where organisms have an extra chromosome 21,
sometimes known as trisomy 21. Being a syndrome, DS consists of multiple symptoms affecting a
large number of systems in the body. It’s effect on learning results in it being an intellectual
disability [1]​. Memantine, is currently proposed as a treatment of the learning deficit symptoms in
DS. In this project, we have used several supervised machine learning methods: a decision tree
classifier, a random forest classifier, and a third classifier which uses a chain of random forest
classifiers., to identify which protein(s) are critical to mice learning ability after being exposed to
context fear conditioning (CFC). 77 protein expression levels are analysed from both control and
trisomic (Ts65Dn) genotype mice, both with and without treatment from the drug memantine.
Result suggest that decision tree and random forest classification approach can identify the most
important proteins which may help to identify more effective drug to help learning process in people
with DS.












INTRODUCTION 

Data Set Information:
The data set consists of the expression levels of 77 proteins/protein modifications that produced detectable signals in the nuclear fraction of cortex. There are 38 control mice and 34 trisomic mice (Down syndrome), for a total of 72 mice. In the experiments, 15 measurements were registered of each protein per sample/mouse. Therefore, for control mice, there are 38x15, or 570 measurements, and for trisomic mice, there are 34x15, or 510 measurements. The dataset contains a total of 1080 measurements per protein. Each measurement can be considered as an independent sample/mouse.

The eight classes of mice are described based on features such as genotype, behavior and treatment. According to genotype, mice can be controlled or trisomic. According to behavior, some mice have been stimulated to learn (context-shock) and others have not (shock-context) and in order to assess the effect of the drug memantine in recovering the ability to learn in trisomic mice, some mice have been injected with the drug and others have not.

Classes:
c-CS-s: control mice, stimulated to learn, injected with saline (9 mice)
c-CS-m: control mice, stimulated to learn, injected with memantine (10 mice)
c-SC-s: control mice, not stimulated to learn, injected with saline (9 mice)
c-SC-m: control mice, not stimulated to learn, injected with memantine (10 mice)
t-CS-s: trisomy mice, stimulated to learn, injected with saline (7 mice)
t-CS-m: trisomy mice, stimulated to learn, injected with memantine (9 mice)
t-SC-s: trisomy mice, not stimulated to learn, injected with saline (9 mice)
t-SC-m: trisomy mice, not stimulated to learn, injected with memantine (9 mice)
The aim is to identify subsets of proteins that are discriminant between the classes.


In this project, 77 expression levels of proteins/protein modifications were examined to see which proteins contributed to successful and failed learning. These proteins produced detectable signals in the nuclear fraction of cortex, and in this research, it gathered from a total of 72 mice. There were 38 control/normal mice and 34 trisomic mice, both trained in context fear conditioning (CFC).The CFC process required these mice to be separated into two groups, context-shock (CS) and shock-context (SC) groups. First, mice from the CS group are placed in a cage, allowed to explore the cage and then given a brief electric shock. Control/normal mice should freeze and learn the association of their cage and the shock, while trisomic mice are supposed to fail to learn. Second, mice in the SC group are placed in a cage and given the electric shock immediately, therefore both normal and trisomicmice will fail to learn the association between cage and the shock.
To assist trisomic mice in learning, memantine is injected prior to training. To control the effect of this injection, half of the mice in the CS and SC group are injected with memantine, while the other groupis injected with saline (no-drugs).

15 measurements of each protein are being conducted. Therefore, there were 15x38 (570 measurements) for control/normal mice, and 15x34 (510 measurements) of trisomic mice. In total,This dataset has 1080 measurements from 72 mice in each expression level of proteins. Therelationship of these data is listed in figure below:




The goal of this project is to understand which trisomy protein classes contribute to the success and the failure of mice learning. This is done by creating a model which predicts which of the 8 classes of mice some mouse was in based on their protein expression levels. By creating a successful model, we can then determine which proteins were significant in the predictions, which would support a hypothesis that that particular protein affects learning in trisomic mice.
