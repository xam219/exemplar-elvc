# Exemplar-Based Methods for Mandarin Electrolaryngeal Speech Voice Conversion

## Abstact
Electrolarynx (EL) can restore speech to patients without vocal cords, but the resulting speech often lacks naturalness and intelligibility. Inspired by recent advances in exemplar-based methods for speaker voice conversion (VC), this study explores their application to electrolaryngeal speech voice conversion (ELVC). As a baseline, we apply the k-nearest neighbors VC (KNN-VC) method with self-supervised learning (SSL) representations to ELVC. To circumvent the SSL feature mismatch between EL speech and natural speech when applying KNN-VC to ELVC, we propose two methods under the parallel VC setting: the parallel KNN-ELVC method and the parallel locally linear embedding (LLE)-based ELVC method. Experimental results demonstrate that while directly applying KNN-VC to ELVC improves the naturalness of EL speech, our proposed methods, especially LLE-ELVC, significantly improve both naturalness and intelligibility. Furthermore, LLE-ELVC is comparable to our previous deep-learning-based ELVC method, further demonstrating the potential of exemplar-based methods in ELVC tasks.

## Reference systems in Table 1

* KNN: the baseline system (in section 2) using dynamic features with K=256
* pKNN: the proposed system (in section 3) using static features with K=8
* LLE: the proposed system (in section 3) using dynamic features with K=256
* CDVAE: the baseline DNN-based ELVC system [^first]
* NLXX: natural speech of speaker ID
* ELXX: electrolaryngeal speech of speaker ID


## Reference

[^first]: Hsin-Hao Chen, Yung-Lun Chien, Ming-Chi Yen, Shu-Wei Tsai, Tai-Shih Chi, Hsin-Min Wang, and Yu Tsao,“Mandarin electrolaryngeal speech voice conversion using cross-domain features,” in Proceedings of INTERSPEECH, 2023, pp. 5018–5022.
