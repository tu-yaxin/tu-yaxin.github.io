---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a third-year PhD student in the [theory group](https://theory.cs.princeton.edu/) in Princeton University, where I am fortunate to be coadvised by Prof. [Alex Lombardi](https://sites.google.com/view/alex-lombardi/home) and Prof. [Ran Raz](https://engineering.princeton.edu/faculty/ran-raz). I'm broadly interested in TCS, with a current focus on cryptography and communication complexity. 

Prior to joining Princeton, I graduated from Yao Class at Tsinghua University. During my undergraduate, I was fortunate to be advised by great people. I was fortunate to work with Prof. [Yilei Chen](http://www.chenyilei.net/) at Tsinghua who sparked my interest in cryptography. During 2022 I had an amazing time at Reichman University and NTT Research working with Prof. [Elette Boyle](https://cs.idc.ac.il/~elette/) and Prof. [Yuval Ishai](https://yuvali.cswp.cs.technion.ac.il/). 



<h2 id="publications"> Publications</h2>

- **On SNARGs, $i\mathcal{O}$, and Falsifiability**  \
  Alex Lombardi, <u>Yaxin Tu</u>, Daniel Wichs  \
  Submitted to Crypto 2026 \
  <details>
  <summary>Abstract</summary> <div style="padding-left: 40px; padding-right: 10px; text-align: justify; color: #6F4E37; max-width: 800px; font-size: 0.8em">
    The Gentry-Wichs barrier (STOC '11) rules out constructions of succinct non-interactive arguments (SNARGs) for $\mathsf{NP}$ with black-box security proofs under falsifiable assumptions. On the other hand, a recent work of Waters and Wu (CRYPTO '25) constructs SNARGs for NP from subexponentially secure indistinguishability obfuscation and one-way functions. This naturally suggests the following two questions: what kinds of SNARG constructions does the Gentry-Wichs technique actually rule out, and is the apparent unfalsifiability of $i\mathcal{O}$ helpful for circumventing Gentry-Wichs?<br><br>
    We provide answers to these questions. First, we prove an impossibility result ruling out $\mathsf{SNARG}$ constructions under assumptions that are ``falsifiable with preprocessing,'' a notion that we introduce. As a consequence, we rule out $\mathsf{SNARG}$ constructions based on polynomially secure $i\mathcal{O}$ and one-way functions. This result is tight in the sense that there are (black-box) constructions of <it>non-adaptively</it> sound $\mathsf{SNARG}$s from these assumptions [Sahai-Waters, STOC '14] and of adaptively sound $\mathsf{SNARG}$s from $i\mathcal{O}$ and one-way functions with a security loss of $2^n$ [Waters-Wu]. Our result proves that this superpolynomial security loss is inherent for black-box reductions. <br><br>
    Second, we extend the original Gentry-Wichs result (and our first result) to the following important setting: (1) the $\mathsf{SNARG}$ candidate has a long common reference string, and (2) the black-box security reduction is allowed to call the adversary on arbitrary choices of security parameter. We prove that any $\mathsf{SNARG}$ with a polynomial-time (or quasi-polynomial time) black-box security reduction based on an assumption $A$ implies that $A$ is broken in <it>quasi</it>-polynomial time. We also observe that existing $\mathsf{SNARG}$ constructions imply that this result is best possible. These two results settle exactly what kinds of adaptive $\mathsf{SNARG}$ constructions are ruled out by Gentry-Wichs style meta-reductions.<br><br>
    Finally, focusing on the special case of indistinguishability obfuscation, we construct a family of oracles relative to which (1) $i\mathcal{O}$ and one-way functions exist, but (2) $i\mathcal{O}$ is black-box equivalent to a falsifiable assumption. This suggests that although $i\mathcal{O}$ is not known to reduce to an efficiently falsifiable assumption, in some settings its power may be limited to that of falsifiable assumptions.
    </div>
  </details>

- **Optimally Succinct Oblivious Transfer via Projective PRGs**  \
  Elette Boyle, Niv Gilboa, Yuval Ishai, Lisa Kohl, Peter Scholl, <u>Yaxin Tu</u>  \
  Submitted to Crypto 2026 \
  <details>
  <summary>Abstract</summary> <div style="padding-left: 40px; padding-right: 10px; text-align: justify; color: #7a8288; max-width: 800px;">
      We identify and explore new connections between highly succinct protocols for oblivious transfer (OT) and projective pseudorandom generators, as recently put forth by Applebaum et al. (STOC 2023).  Leveraging these connections, we improve the communication cost of OT and related primitives, obtaining the following results:
  <ol>
      <li> Chosen-Receiver OTs with $O(1)$ Group Elements. Based on either strong RSA or bilinear maps, we are the first to realize $n$ random OTs by communicating only a {\em constant} number of group elements. With the same communication, our protocol further supports random sender inputs and {\em chosen} receiver inputs.
      Our protocols enable setting up base OTs for a variety of applications with a much lower communication cost compared to existing protocols, at a moderate additional (or even similar) computation~cost. </li>
  <li>Practical Rate-1 OT/OLE from Groups. Building on the previous protocols, we obtain the first concretely efficient "rate-1" batch OT, from standard group-based assumptions. Our protocols realize $n$ bit-OTs with $2n+o(n)$ bits of communication, are black-box in the underlying cryptographic tools, and provide typical throughput of up to thousands of OTs per second on a single CPU core. Our protocols also generalize to achieve rate-1 OLE over $\mathbb{Z}_m$ for a smooth modulus $m$. </li>
  </ol>
      Our pairing-based protocol is based on a new, succinct flavor of VOLE, which beyond OT, can be used to improve the communication cost of private set intersection (PSI).
    </div>
  </details>

- **LWE with Quantum Amplitudes: Algorithm, Hardness, and Oblivious Sampling**  \
  Yilei Chen, Zihan Hu, Qipeng Liu, Han Luo, <u>Yaxin Tu</u>  \
  Crypto 2025 \
  [ePrint](https://eprint.iacr.org/2023/1498), [arXiv](https://arxiv.org/abs/2310.00644) \
  <details>
  <summary>Abstract</summary> <div style="padding-left: 40px; padding-right: 10px; text-align: justify; color: #7a8288; max-width: 800px;">
      The learning with errors problem (LWE) is one of the most important building blocks for post-quantum cryptography. To better understand the quantum hardness of LWE, it is crucial to explore quantum variants of LWE. To this end, Chen, Liu, and Zhandry [Eurocrypt 2022] defined S|LWE⟩ and C|LWE⟩ problems by encoding the error of LWE samples into quantum amplitudes, and showed efficient quantum algorithms for a few interesting amplitudes. However, algorithms or hardness results of the most interesting amplitude, Gaussian, were not addressed before.<br><br>
      In this paper, we show new algorithms, hardness results and applications for S|LWE⟩ and S|LWE⟩ with real Gaussian, Gaussian with linear or quadratic phase terms, and other related amplitudes. Let n be the dimension, q be the modulus of LWE samples. Our main results are
  <ol>
      <li>
        There is a $2^{\Theta(\sqrt{n\log q})}$-time algorithm for S|LWE⟩ with Gaussian amplitude with known phase, given $2^{\Theta(\sqrt{n\log q})}$ many quantum samples. The algorithm is modified from Kuperberg's sieve, and in fact works for more general amplitudes as long as the amplitudes and phases are completely known.
      </li>
      <li>
        There is a polynomial time quantum algorithm for solving S|LWE⟩ and C|LWE⟩ for Gaussian with quadratic phase amplitudes, where the sample complexity is as small as $\tilde{O}(n)$. As an application, we give a quantum oblivious LWE sampler where the core quantum sampler requires only quasi-linear sample complexity. This improves upon the previous oblivious LWE sampler given by Debris-Alazard, Fallahpour, Stehlé [STOC 2024], whose core quantum sampler requires $\tilde{O}(nr)$ sample complexity, where r is the standard deviation of the error.
      </li>
      <li>
        There exist polynomial time quantum reductions from standard LWE or worst-case GapSVP to S|LWE⟩ with Gaussian amplitude with small unknown phase, and arbitrarily many samples. Compared to the first two items, the appearance of the unknown phase term places a barrier in designing efficient quantum algorithm for solving standard LWE via S|LWE⟩.
      </li>
    </ol>
    </div>
  </details>

- **Improved Constructions for Distributed Multi-Point Functions**  \
  Elette Boyle, Niv Gilboa, Matan Hamilis, Yuval Ishai, <u>Yaxin Tu</u>  \
  IEEE Symposium on Security and Privacy 2025 \
  [Link](https://doi.ieeecomputersociety.org/10.1109/SP61157.2025.00044) \
  <details>
  <summary>Abstract</summary> <div style="padding-left: 40px; padding-right: 10px; text-align: justify; color: #7a8288; max-width: 800px;">
      A Distributed Point Function (DPF) is a cryptographic primitive used for compressing additive secret shares of a secret unit vector across two parties. Many DPF applications require compressed shares of a sparse <i>weight-t</i> vector, namely a Distributed Multi-Point Function (DMPF). Despite the strong motivation and prior optimization efforts, in most use cases the best practical implementation of DMPF is still a simple brute-force combination of t independent DPFs. <br><br>
      We present new constructions and optimized implementations of DMPFs in different parameter regimes, providing significant efficiency savings over existing approaches. We showcase our new constructions within applications of pseudorandom correlation generators (PCGs) and 2-server private set intersection (PSI). <br><br>
      Incorporating our tools into the state-of-the-art PCG for “silent” generation of binary multiplication triples (FOLEAGE, Bombar et al, ePrint’24) yields a ×2.68 improvement in throughput, with only ×1.4 blowup in the seed size. On a single core of our benchmark machine, our implementation silently generates up to 22.1 million triples per second, outperforming even the best “non-silent” protocol (Roy, CRYPTO’22), which generates 16 million triples per second.
    </div>
  </details>

- **A Modal Approach Towards Substitutions**   \
  <u>Yaxin Tu</u>, Sujata Ghosh, Fenrong Liu, Dazhu Li \
  Annals of Pure and Applied Logic, Volume 177 \
  [Link](https://doi.org/10.1016/j.apal.2026.103742)  \
  <details>
  <summary>Abstract</summary> <div style="padding-left: 40px; padding-right: 10px; text-align: justify; color: #7a8288; max-width: 800px;">
  Substitutions play a crucial role in a wide range of contexts, from analyzing the dynamics of social opinions and conducting mathematical computations to engaging in game-theoretical analysis. For many situations, considering one-step substitutions is often adequate. Yet, for more complex cases, iterative substitutions become indispensable. In this article, our primary focus is to study logical frameworks that model both single-step and iterative substitutions. We explore a number of properties of these logics, including their expressive strength, Hilbert-style proof systems, and satisfiability problems. Additionally, we establish connections between our proposed frameworks and relevant existing ones in the literature. For instance, we precisely delineate the relationship between single-step substitutions and the standard syntactic replacements commonly found in many classical logics. Moreover, special emphasis is placed on iterative substitutions. In this context, we compare our proposed framework with existing ones involving iterative reasoning, thereby highlighting the advantages of our proposal. </div>
  </details>

- **A Simple Logic of the Hide and Seek Game**   \
  Dazhu Li, Sujata Ghosh, Fenrong Liu, <u>Yaxin Tu</u>  \
  Studia Logica, Volume 111 \
  [Link](https://link.springer.com/article/10.1007/s11225-023-10039-4)  \
  <details>
  <summary>Abstract</summary> <div style="padding-left: 40px; padding-right: 10px; text-align: justify; color: #7a8288; max-width: 800px;">
  We discuss a simple logic to describe one of our favourite games from childhood, hide and seek, and show how a simple addition of an equality constant to describe the winning condition of the seeker makes our logic undecidable. There are certain decidable fragments of first-order logic which behave in a similar fashion with respect to such a language extension, and we add a new modal variant to that class. We discuss the relative expressive power of the proposed logic in comparison to the standard modal counterparts. We prove that the model checking problem for the resulting logic is P-complete. In addition, by exploring the connection with related product logics, we gain more insight towards having a better understanding of the subtleties of the proposed framework.</div>
  </details>

- **On the Subtle Nature of a Simple Logic of the Hide and Seek Game**  \
  Dazhu Li, Sujata Ghosh, Fenrong Liu, <u>Yaxin Tu</u>  \
  WoLLIC 2021  \
  [Link](https://link.springer.com/chapter/10.1007/978-3-030-88853-4_13) \ 
  <details>
  <summary>Abstract</summary> <div style="padding-left: 40px; padding-right: 10px; text-align: justify; color: #7a8288; max-width: 800px;">
  We discuss a simple logic to describe one of our favourite games from childhood, hide and seek, and show how a simple addition of an equality constant to describe the winning condition of the seeker makes our logic undecidable. There are certain decidable fragments of first-order logic which behave in a similar fashion and we add a new modal variant to that class of logics. We also discuss the relative expressive power of the proposed logic in comparison to the standard modal counterparts.</div>
  </details>

<h2 id="teaching"> Teaching</h2>
- (Fall 2025) TA for COS 585: Information Theory by Prof. Ran Raz, Princeton University

- (Fall 2024) TA for [COS 433/533: Cryptography](https://sites.google.com/view/alex-lombardi/home/cos-433533-fall-2024-princeton) by Prof. Alex Lombardi, Princeton University

- (Spring 2023) TA for Secure Multiparty Computation: Theory and Application by Prof. Yifan Song, Tsinghua University

<h2 id="experience"> Experience</h2>
- Research intern in [FACT Center](https://www.factcenter.org/) hosted by Prof. Elette Boyle, Reichman University (Feb 2022 - Aug 2022)
