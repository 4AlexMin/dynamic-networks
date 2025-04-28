# Dynamic Network Datasets

This repository contains a structured collection of **dynamic (temporal) network datasets**, organized for network behavior analysis research.

Each dataset records the interactions or connections between entities (nodes) over time.  
The data is formatted as plain text files, where **each line represents a temporal edge** in the form:

```plaintext
nodeA  nodeB  timestamp
```

Datasets are grouped into two types:
- **50 Human-based Networks**: Interactions between people or human-generated data.
- **29 Non-human (animal) Networks**: Interactions observed among animals or biological entities.

Each type is further organized into logical categories based on network characteristics to facilitate research and analysis.


---

## 📁 Folder Structure
```plaintext
organized_data/
├── human/
│   ├── Citation Networks/
│   ├── Communication Networks/
│   ├── Interactive Digital Communities/
│   ├── Recommendation Networks/
│   ├── Physical Contacts/
│   └── Others/
└── non-human/
    ├── aves/
    ├── insecta/
    ├── mammalia/
    └── reptilia/
```

---

## 🗃️ Dataset Overview


### Human Networks

This collection of 50 human dynamic networks were acquired and structured from well-established public data repositories, including [SNAP](https://snap.stanford.edu/), [Network Repository](http://networkrepository.com/), [SocioPatterns](http://www.sociopatterns.org/), [WoSNet](http://wosnproject.org/), and datasets collected by [Opsahl et al](https://doi.org/10.1016/j.socnet.2009.02.002).  


| Network | #Nodes ($N$) | #Edges ($E$) | $E/N$ | Average Degree | Network Density | Source |
|:---|---:|---:|---:|---:|---:|:---|
| **Category: Citation Networks** |||||||
| cit-HepPh | 30,566 | 347,414 | 11.37 | 22.73 | $7.40\times10^{-4}$ | SNAP |
| cit-HepTh | 18,477 | 136,427 | 7.38 | 14.77 | $8.00\times10^{-4}$ | SNAP |
| cit-Patents-DK | 28,873 | 29,988 | 1.04 | 2.08 | $7.00\times10^{-5}$ | SNAP |
| cit-Patents-ES | 17,998 | 17,027 | 0.95 | 1.89 | $1.10\times10^{-4}$ | SNAP |
| cit-Patents-IL | 46,986 | 55,935 | 1.19 | 2.38 | $5.00\times10^{-5}$ | SNAP |
| cit-Patents-SU | 21,719 | 19,964 | 0.92 | 1.84 | $8.00\times10^{-5}$ | SNAP |
| **Category: Interactive Digital Communities** |||||||
| digg-friends | 279,374 | 1,729,983 | 6.19 | 12.38 | $4.00\times10^{-5}$ | Network Repository |
| fbno-walls | 46,952 | 876,993 | 18.68 | 37.36 | $8.00\times10^{-4}$ | WoSNet |
| ia-chess-combined | 7,301 | 65,053 | 8.91 | 17.82 | $2.44\times10^{-3}$ | Network Repository |
| rec-stackoverflow | 545,196 | 1,301,942 | 2.39 | 4.78 | $1.00\times10^{-5}$ | Network Repository |
| sx-askubuntu | 159,316 | 964,437 | 6.05 | 12.11 | $8.00\times10^{-5}$ | SNAP |
| sx-askubuntu-a2q | 137,517 | 280,102 | 2.04 | 4.07 | $3.00\times10^{-5}$ | SNAP |
| sx-askubuntu-c2a | 75,555 | 356,822 | 4.72 | 9.45 | $1.30\times10^{-4}$ | SNAP |
| sx-askubuntu-c2q | 79,155 | 327,513 | 4.14 | 8.28 | $1.00\times10^{-4}$ | SNAP |
| sx-mathoverflow | 24,818 | 506,550 | 20.41 | 40.82 | $1.64\times10^{-3}$ | SNAP |
| sx-mathoverflow-a2q | 21,688 | 107,581 | 4.96 | 9.92 | $4.60\times10^{-4}$ | SNAP |
| sx-mathoverflow-c2a | 13,840 | 195,330 | 14.11 | 28.23 | $2.04\times10^{-3}$ | SNAP |
| sx-mathoverflow-c2q | 16,836 | 203,639 | 12.10 | 24.19 | $1.44\times10^{-3}$ | SNAP |
| sx-superuser | 194,085 | 1,443,339 | 7.44 | 14.87 | $8.00\times10^{-5}$ | SNAP |
| sx-superuser-a2q | 167,981 | 430,033 | 2.56 | 5.12 | $3.00\times10^{-5}$ | SNAP |
| sx-superuser-c2a | 101,052 | 534,239 | 5.29 | 10.57 | $1.00\times10^{-4}$ | SNAP |
| sx-superuser-c2q | 94,548 | 479,067 | 5.07 | 10.13 | $1.10\times10^{-4}$ | SNAP |
| **Category: Communication Networks** |||||||
| CollegeMsg | 1,899 | 59,835 | 31.51 | 63.02 | $3.32\times10^{-2}$ | SNAP/Opsahl |
| email-Eu-Dept1 | 309 | 61,046 | 197.56 | 395.12 | $1.28$ | SNAP |
| email-Eu-Dept2 | 162 | 46,772 | 288.72 | 577.43 | $3.59$ | SNAP |
| email-Eu-Dept3 | 89 | 12,216 | 137.26 | 274.52 | $3.12$ | SNAP |
| email-Eu-Dept4 | 142 | 48,141 | 339.02 | 678.04 | $4.81$ | SNAP |
| email-Eu-core-temporal | 986 | 332,334 | 337.05 | 674.11 | $6.84\times10^{-1}$ | SNAP |
| email-dnc | 1,891 | 39,264 | 20.76 | 41.53 | $2.20\times10^{-2}$ | Network Repository |
| ia-reality-call | 6,809 | 52,050 | 7.64 | 15.29 | $2.25\times10^{-3}$ | Network Repository |
| ia-retweet-pol | 18,470 | 61,157 | 3.31 | 6.62 | $3.60\times10^{-4}$ | Network Repository |
| tech-as-topology | 34,761 | 171,403 | 4.93 | 9.86 | $2.80\times10^{-4}$ | Network Repository |
| **Category: Recommendation Networks** |||||||
| soc-epinion-combined | 131,828 | 841,372 | 6.38 | 12.76 | $1.00\times10^{-4}$ | Network Repository |
| soc-epinion-neg | 43,347 | 123,705 | 2.85 | 5.71 | $1.30\times10^{-4}$ | Network Repository |
| soc-epinion-pos | 114,467 | 717,667 | 6.27 | 12.54 | $1.10\times10^{-4}$ | Network Repository |
| soc-sign-bitcoin-alpha | 3,783 | 24,186 | 6.39 | 12.79 | $3.38\times10^{-3}$ | SNAP |
| soc-sign-bitcoin-otc | 5,881 | 35,592 | 6.05 | 12.10 | $2.06\times10^{-3}$ | SNAP |
| soc-wiki-elec-combined | 7,118 | 107,071 | 15.04 | 30.08 | $4.23\times10^{-3}$ | Network Repository |
| soc-wiki-elec-neg | 4,223 | 23,118 | 5.47 | 10.95 | $2.59\times10^{-3}$ | Network Repository |
| soc-wiki-elec-pos | 6,271 | 83,953 | 13.39 | 26.77 | $4.27\times10^{-3}$ | Network Repository |
| **Category: Physical Contacts** |||||||
| SFHH-conf | 403 | 70,261 | 174.34 | 348.69 | $8.67\times10^{-1}$ | SocioPatterns |
| hypertext-conf | 113 | 20,818 | 184.23 | 368.46 | $3.29$ | SocioPatterns |
| ia-contacts_dublin | 10,972 | 415,912 | 37.91 | 75.81 | $6.91\times10^{-3}$ | Network Repository |
| infectious-conf | 410 | 17,298 | 42.19 | 84.38 | $2.06\times10^{-1}$ | Network Repository |
| **Category: Others** |||||||
| fbno-links | 61,096 | 905,565 | 14.82 | 29.64 | $4.90\times10^{-4}$ | WoSNet |
| high-school-2011 | 126 | 28,561 | 226.67 | 453.35 | $3.63$ | SocioPatterns |
| high-school-2012 | 180 | 45,047 | 250.26 | 500.52 | $2.80$ | SocioPatterns |
| high-school-2013 | 327 | 188,508 | 576.48 | 1,152.95 | $3.54$ | SocioPatterns |
| ia-frwikinews-user-edits | 25,042 | 193,618 | 7.73 | 15.46 | $6.20\times10^{-4}$ | Network Repository |
| primary-school | 242 | 125,773 | 519.72 | 1,039.45 | $4.31$ | SocioPatterns |



---

### Non-Human Networks



This collection includes 29 dynamic networks spanning four major Linnaean classes: *Mammalia*, *Aves*, *Reptilia*, and *Insecta*.  
The datasets were primarily sourced from the [ASNR repository](https://bansallab.github.io/asnr/data.html) and **manually collected and formatted** from published animal behavior research articles.

- **Aves**:  
  Bird social networks, including wildbirds, weavers, parakeets, and sparrows.

- **Insecta**:  
  Ant colony interaction and trophallaxis (food-sharing) networks.

- **Mammalia**:  
  Mammal social behavior networks, including elephant seals, bats, voles, raccoons, and primates.

- **Reptilia**:  
  Tortoise social interaction networks.

---

## 📜 License


The code, organization scripts, and documentation in this repository are licensed under the **MIT License**.

**Important Note**:  
The datasets included in this repository are sourced from third-party public repositories, each of which may have their own licensing terms.  
In particular, datasets from [SocioPatterns](http://www.sociopatterns.org/) are subject to a **Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)**.  
Users must comply with the original licenses when using any dataset provided here.

License Details: [LICENSE](./LICENSE)

<!-- --- -->
<!-- 
## 📋 Third-Party Dataset Sources

This repository organizes datasets collected from the following sources:

- [SNAP: Stanford Large Network Dataset Collection](https://snap.stanford.edu/)
- [Network Repository](http://networkrepository.com/)
- [SocioPatterns](http://www.sociopatterns.org/)
- [WoSNet (World of Science Networks)](http://wosnproject.org/)
- Public repositories of various academic papers

Please refer to the original sources for specific licensing or citation requirements related to the original datasets.

--- -->

<!-- ## ✏️ Citation

If you find this dataset collection useful in your research, please cite this repository: -->