---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a second-year PhD student in the [theory group](https://theory.cs.princeton.edu/) in Princeton University, where I am fortunate to be coadvised by Prof. [Ran Raz](https://engineering.princeton.edu/faculty/ran-raz) and Prof. [Alex Lombardi](https://sites.google.com/view/alex-lombardi/home). I have found and am exploring my interests broadly in TCS, including complexity theory, cryptography, and their interplay. 

Prior to joining Princeton, I graduated from Yao Class at Tsinghua University. During my undergraduate, I was fortunate to be advised by great people. I was fortunate to work with Prof. [Yilei Chen](http://www.chenyilei.net/) at Tsinghua who sparked my interest in cryptography. During 2022 I had an amazing time at Reichman University and NTT Research working with Prof. [Elette Boyle](https://cs.idc.ac.il/~elette/) and Prof. [Yuval Ishai](https://yuvali.cswp.cs.technion.ac.il/). 



<h2 id="publications"> Publications</h2>

- **Improved Constructions for Distributed Multi-Point Functions**  \
  Elette Boyle, Niv Gilboa, Matan Hamilis, Yuval Ishai, *Yaxin Tu*  \
  IEEE Symposium on Security and Privacy 2025 \
  <details>
  <summary>Abstract</summary> <span style="padding-left: 40px; padding-right: 10px; text-align: justify; color: #7a8288;">
  A Distributed Point Function (DPF) is a cryptographic primitive used for compressing additive secret shares of a secret unit vector across two parties. Many DPF applications require compressed shares of a sparse <i>weight-t</i> vector, namely a Distributed Multi-Point Function (DMPF). Despite the strong motivation and prior optimization efforts, in most use cases the best practical implementation of DMPF is still a simple brute-force combination of t independent DPFs. </span><br>

  <span style="padding-left: 40px;color:#7a8288;">We present new constructions and optimized implementations of DMPFs in different parameter regimes, providing significant efficiency savings over existing approaches. We showcase our new constructions within applications of pseudorandom correlation generators (PCGs) and 2-server private set intersection (PSI). </span><br>

  <span style="padding-left: 40px;color:#7a8288;">Incorporating our tools into the state-of-the-art PCG for “silent” generation of binary multiplication triples (FOLEAGE, Bombar et al, ePrint’24) yields a ×2.68 improvement in throughput, with only ×1.4 blowup in the seed size. On a single core of our benchmark machine, our implementation silently generates up to 22.1 million triples per second, outperforming even the best “non-silent” protocol (Roy, CRYPTO’22), which generates 16 million triples per second. </span>
  </details>
  [Link](https://doi.ieeecomputersociety.org/10.1109/SP61157.2025.00044) 

- **LWE with Quantum Amplitudes: Algorithm, Hardness, and Oblivious Sampling**  \
  Yilei Chen, Zihan Hu, Qipeng Liu, Han Luo, *Yaxin Tu*  \
  [Eprint](https://eprint.iacr.org/2023/1498), [arXiv](https://arxiv.org/abs/2310.00644) 

- **A Simple Logic of the Hide and Seek Game**   \
  Dazhu Li, Sujata Ghosh, Fenrong Liu, *Yaxin Tu*  \
  Studia Logica Volume 111  \
  <details>
  <summary>Abstract</summary> <span style="padding-left: 40px;color:#7a8288;">
  We discuss a simple logic to describe one of our favourite games from childhood, hide and seek, and show how a simple addition of an equality constant to describe the winning condition of the seeker makes our logic undecidable. There are certain decidable fragments of first-order logic which behave in a similar fashion with respect to such a language extension, and we add a new modal variant to that class. We discuss the relative expressive power of the proposed logic in comparison to the standard modal counterparts. We prove that the model checking problem for the resulting logic is P-complete. In addition, by exploring the connection with related product logics, we gain more insight towards having a better understanding of the subtleties of the proposed framework.</span>
  </details>
  [Link](https://link.springer.com/article/10.1007/s11225-023-10039-4) 

- **On the Subtle Nature of a Simple Logic of the Hide and Seek Game**  \
  Dazhu Li, Sujata Ghosh, Fenrong Liu, *Yaxin Tu*  \
  WoLLIC 2021  \
  <details>
  <summary>Abstract</summary> <span style="padding-left: 40px;color:#7a8288;">
  We discuss a simple logic to describe one of our favourite games from childhood, hide and seek, and show how a simple addition of an equality constant to describe the winning condition of the seeker makes our logic undecidable. There are certain decidable fragments of first-order logic which behave in a similar fashion and we add a new modal variant to that class of logics. We also discuss the relative expressive power of the proposed logic in comparison to the standard modal counterparts.</span>
  </details>
  [Link](https://link.springer.com/chapter/10.1007/978-3-030-88853-4_13)  

<h2 id="teaching"> Teaching</h2>
- (Fall 2024) TA for [Cryptography](https://sites.google.com/view/alex-lombardi/home/cos-433533-fall-2024-princeton) by Prof. Alex Lombardi, Princeton University

- (Spring 2023) TA for Secure Multiparty Computation: Theory and Application by Prof. Yifan Song, Tsinghua University

<h2 id="experience"> Experience</h2>
- Research intern in [FACT Center](https://www.factcenter.org/) hosted by Prof. Elette Boyle, Reichman University (Feb 2022 - Aug 2022)
