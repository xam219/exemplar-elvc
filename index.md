# Exemplar-Based Methods for Mandarin Electrolaryngeal Speech Voice Conversion

## Abstact
Electrolarynx (EL) can restore speech to patients without vocal cords, but the resulting speech often lacks naturalness and intelligibility. Inspired by recent advances in exemplar-based methods for speaker voice conversion (VC), this study explores their application to electrolaryngeal speech voice conversion (ELVC). As a baseline, we apply the k-nearest neighbors VC (KNN-VC) method with self-supervised learning (SSL) representations to ELVC. To circumvent the SSL feature mismatch between EL speech and natural speech when applying KNN-VC to ELVC, we propose two methods under the parallel VC setting: the parallel KNN-ELVC method and the parallel locally linear embedding (LLE)-based ELVC method. Experimental results demonstrate that while directly applying KNN-VC to ELVC improves the naturalness of EL speech, our proposed methods, especially LLE-ELVC, significantly improve both naturalness and intelligibility. Furthermore, LLE-ELVC is comparable to our previous deep-learning-based ELVC method, further demonstrating the potential of exemplar-based methods in ELVC tasks.

## Reference systems in Table 1

* __KNN-ELVC-d__: the baseline system (in section 2) using dynamic features with K=256
* __pKNN-ELVC-s__: the proposed system (in section 3) using static features with K=8
* __LLE-ELVC-d__: the proposed system (in section 3) using dynamic features with K=256
* __CDVAE__: the baseline DNN-based ELVC system [^first]
* NLXX: natural speech of speaker ID
* ELXX: electrolaryngeal speech of speaker ID

## Audio samples

**241**

|   System   | transcription: 再十分鐘火車就要開了 (zai shi fen zhong huo che jiu yao kai le) | 
|:---------:|:-------------------------------------------------------------------:|
| EL speech | <audio src="audio/EL01v3_audio_segment_16k/EL01v3_241.wav" controls preload></audio> |
| __KNN-ELVC-d__  | <audio src="audio/knnvc_dynamic_mlpg_k256/241.wav" controls preload></audio> |
| __pKNN-ELVC-s__  | <audio src="audio/knnvc_static_parallel_k8/241.wav" controls preload></audio> |
| __LLE-ELVC-d__  | <audio src="audio/llevc_dynamic_k256/241.wav" controls preload></audio> |
| __CDVAE__ | <audio src="audio/cdvae_vocoder_prematch/EL01v3_NL01v3_241.wav" controls preload></audio> |
| NL speech | <audio src="audio/NL01v3_audio_segment_16k/NL01v3_241.wav" controls preload></audio> |

**242**

|   System   | transcription: 哥哥的腳長了個大水泡 (ge ge de jiao zhang le ge da shui pao) | 
|:---------:|:-------------------------------------------------------------------:|
| EL speech | <audio src="audio/EL01v3_audio_segment_16k/EL01v3_242.wav" controls preload></audio> |
| __KNN-ELVC-d__  | <audio src="audio/knnvc_dynamic_mlpg_k256/242.wav" controls preload></audio> |
| __pKNN-ELVC-s__  | <audio src="audio/knnvc_static_parallel_k8/242.wav" controls preload></audio> |
| __LLE-ELVC-d__   | <audio src="audio/llevc_dynamic_k256/242.wav" controls preload></audio> |
| __CDVAE__ | <audio src="audio/cdvae_vocoder_prematch/EL01v3_NL01v3_242.wav" controls preload></audio> |
| NL speech | <audio src="audio/NL01v3_audio_segment_16k/NL01v3_242.wav" controls preload></audio> |

**243**

|   System   | transcription: 醫院大門口有很多花店 (yi yuan da men kou you hen duo hua dian) | 
|:---------:|:-------------------------------------------------------------------:|
| EL speech | <audio src="audio/EL01v3_audio_segment_16k/EL01v3_243.wav" controls preload></audio> |
| __KNN-ELVC-d__  | <audio src="audio/knnvc_dynamic_mlpg_k256/243.wav" controls preload></audio> |
| __pKNN-ELVC-s__  | <audio src="audio/knnvc_static_parallel_k8/243.wav" controls preload></audio> |
| __LLE-ELVC-d__   | <audio src="audio/llevc_dynamic_k256/243.wav" controls preload></audio> |
| __CDVAE__ | <audio src="audio/cdvae_vocoder_prematch/EL01v3_NL01v3_243.wav" controls preload></audio> |
| NL speech | <audio src="audio/NL01v3_audio_segment_16k/NL01v3_243.wav" controls preload></audio> |

**244**

|   System   | transcription: 他們經常去餐廳吃晚飯 (ta men jing chang qu can ting chi wan fan) | 
|:---------:|:-------------------------------------------------------------------:|
| EL speech | <audio src="audio/EL01v3_audio_segment_16k/EL01v3_244.wav" controls preload></audio> |
| __KNN-ELVC-d__  | <audio src="audio/knnvc_dynamic_mlpg_k256/244.wav" controls preload></audio> |
| __pKNN-ELVC-s__  | <audio src="audio/knnvc_static_parallel_k8/244.wav" controls preload></audio> |
| __LLE-ELVC-d__   | <audio src="audio/llevc_dynamic_k256/244.wav" controls preload></audio> |
| __CDVAE__ | <audio src="audio/cdvae_vocoder_prematch/EL01v3_NL01v3_244.wav" controls preload></audio> |
| NL speech | <audio src="audio/NL01v3_audio_segment_16k/NL01v3_244.wav" controls preload></audio> |

**245**

|   System   | transcription: 叔叔家養了一大缸金魚 (shu shu jia yang le yi da gang jin yu) | 
|:---------:|:-------------------------------------------------------------------:|
| EL speech | <audio src="audio/EL01v3_audio_segment_16k/EL01v3_245.wav" controls preload></audio> |
| __KNN-ELVC-d__  | <audio src="audio/knnvc_dynamic_mlpg_k256/245.wav" controls preload></audio> |
| __pKNN-ELVC-s__  | <audio src="audio/knnvc_static_parallel_k8/245.wav" controls preload></audio> |
| __LLE-ELVC-d__   | <audio src="audio/llevc_dynamic_k256/245.wav" controls preload></audio> |
| __CDVAE__ | <audio src="audio/cdvae_vocoder_prematch/EL01v3_NL01v3_245.wav" controls preload></audio> |
| NL speech | <audio src="audio/NL01v3_audio_segment_16k/NL01v3_245.wav" controls preload></audio> |

**316**

|   System   | transcription: 他做完功課才上床睡覺 (ta zuo wan gong ke cai shang chuang shui jue) | 
|:---------:|:-------------------------------------------------------------------:|
| EL speech | <audio src="audio/EL01v3_audio_segment_16k/EL01v3_316.wav" controls preload></audio> |
| __KNN-ELVC-d__  | <audio src="audio/knnvc_dynamic_mlpg_k256/316.wav" controls preload></audio> |
| __pKNN-ELVC-s__  | <audio src="audio/knnvc_static_parallel_k8/316.wav" controls preload></audio> |
| __LLE-ELVC-d__   | <audio src="audio/llevc_dynamic_k256/316.wav" controls preload></audio> |
| __CDVAE__ | <audio src="audio/cdvae_vocoder_prematch/EL01v3_NL01v3_316.wav" controls preload></audio> |
| NL speech | <audio src="audio/NL01v3_audio_segment_16k/NL01v3_316.wav" controls preload></audio> |

**317**

|   System   | transcription: 一群孩子在那邊玩跳繩 (yi qun hai zi zai na bian wan tiao sheng) | 
|:---------:|:-------------------------------------------------------------------:|
| EL speech | <audio src="audio/EL01v3_audio_segment_16k/EL01v3_317.wav" controls preload></audio> |
| __KNN-ELVC-d__  | <audio src="audio/knnvc_dynamic_mlpg_k256/317.wav" controls preload></audio> |
| __pKNN-ELVC-s__  | <audio src="audio/knnvc_static_parallel_k8/317.wav" controls preload></audio> |
| __LLE-ELVC-d__   | <audio src="audio/llevc_dynamic_k256/317.wav" controls preload></audio> |
| __CDVAE__ | <audio src="audio/cdvae_vocoder_prematch/EL01v3_NL01v3_317.wav" controls preload></audio> |
| NL speech | <audio src="audio/NL01v3_audio_segment_16k/NL01v3_317.wav" controls preload></audio> |

**318**

|   System   | transcription: 這裡的風俗習慣很特別 (zhe li de feng su xi guan hen te bie) | 
|:---------:|:-------------------------------------------------------------------:|
| EL speech | <audio src="audio/EL01v3_audio_segment_16k/EL01v3_318.wav" controls preload></audio> |
| __KNN-ELVC-d__  | <audio src="audio/knnvc_dynamic_mlpg_k256/318.wav" controls preload></audio> |
| __pKNN-ELVC-s__  | <audio src="audio/knnvc_static_parallel_k8/318.wav" controls preload></audio> |
| __LLE-ELVC-d__   | <audio src="audio/llevc_dynamic_k256/318.wav" controls preload></audio> |
| __CDVAE__ | <audio src="audio/cdvae_vocoder_prematch/EL01v3_NL01v3_318.wav" controls preload></audio> |
| NL speech | <audio src="audio/NL01v3_audio_segment_16k/NL01v3_318.wav" controls preload></audio> |

**319**

|   System   | transcription: 他腰痛的老毛病又犯了 (ta yao tong de lao mao bing you fan le) | 
|:---------:|:-------------------------------------------------------------------:|
| EL speech | <audio src="audio/EL01v3_audio_segment_16k/EL01v3_319.wav" controls preload></audio> |
| __KNN-ELVC-d__  | <audio src="audio/knnvc_dynamic_mlpg_k256/319.wav" controls preload></audio> |
| __pKNN-ELVC-s__  | <audio src="audio/knnvc_static_parallel_k8/319.wav" controls preload></audio> |
| __LLE-ELVC-d__   | <audio src="audio/llevc_dynamic_k256/319.wav" controls preload></audio> |
| __CDVAE__ | <audio src="audio/cdvae_vocoder_prematch/EL01v3_NL01v3_319.wav" controls preload></audio> |
| NL speech | <audio src="audio/NL01v3_audio_segment_16k/NL01v3_319.wav" controls preload></audio> |

**320**

|   System   | transcription: 他不小心把茶杯碰翻了 (ta bu xiao xin ba cha bei peng fan le) | 
|:---------:|:-------------------------------------------------------------------:|
| EL speech | <audio src="audio/EL01v3_audio_segment_16k/EL01v3_320.wav" controls preload></audio> |
| __KNN-ELVC-d__  | <audio src="audio/knnvc_dynamic_mlpg_k256/320.wav" controls preload></audio> |
| __pKNN-ELVC-s__  | <audio src="audio/knnvc_static_parallel_k8/320.wav" controls preload></audio> |
| __LLE-ELVC-d__   | <audio src="audio/llevc_dynamic_k256/320.wav" controls preload></audio> |
| __CDVAE__ | <audio src="audio/cdvae_vocoder_prematch/EL01v3_NL01v3_320.wav" controls preload></audio> |
| NL speech | <audio src="audio/NL01v3_audio_segment_16k/NL01v3_320.wav" controls preload></audio> |

## Reference

[^first]: Hsin-Hao Chen, Yung-Lun Chien, Ming-Chi Yen, Shu-Wei Tsai, Tai-Shih Chi, Hsin-Min Wang, and Yu Tsao,“Mandarin electrolaryngeal speech voice conversion using cross-domain features,” in Proceedings of INTERSPEECH, 2023, pp. 5018–5022.
