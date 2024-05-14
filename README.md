# Audio Tokenization and Reconstruction

## Introduction

In this demo, we present our latest research results on audio tokenization and the subsequent reconstruction of audio based on those tokens. The process involves converting audio into a series of tokens and then using these tokens to reconstruct the original audio.

### The audio tokenizer works for any speaker, any audio length.
### The audio tokenzier is also SOTA in audio compression

Notice that we are using a rather simple model, primarily trained on ZH dataset, and the output quality can be significantly improve.

## Original Audio

First, let's play the original audio for three samples. All audio samples are randomly picked from websites and datasets that are not used in training.

Original Audio Sample 1 (Zero/One Shot):

<audio controls>
  <source src="audio/speaker.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

Original Audio Sample 2 (Zero Shot):

<audio controls>
  <source src="audio/nana_1.mp3" type="audio/mp3">
  Your browser does not support the audio element.
</audio>

Original Audio Sample 3 (Zero Shot):

<audio controls>
  <source src="audio/speaker_female.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>

## Audio Tokens

Below are the token representations of the original audio samples. The tokens are displayed in dropdown blocks since they can be quite long.

<details>
<summary>Show Tokens for Sample 1</summary>

```text
tensor([[ 9071, 22264, 25096, 23154,  2660, 31228, 11365, 14549, 14565,  7598,
         15033,  7395, 23216, 19608, 30566, 14582, 55354, 22587, 21067, 56648,
         23699, 40150,  7663, 19618, 19892, 26784, 18604, 18856, 59688, 51516,
         26808, 20470, 40746, 61426, 52399, 35258, 52268, 43272, 61555, 41423,
         47595, 39093, 64256, 37526, 43118, 39526, 39654, 47501, 64638, 63596,
         11236,  6370, 36512, 41038, 47990, 55415, 39523,   359,  2230,  7402,
         44065, 61224, 15003, 15046, 10791, 41390, 53631, 31348, 60509, 63610,
         10452, 37609, 23666, 53995,  6384, 55418, 43662,  6196, 44584, 22399,
         21451, 19959, 19624, 51080,  4299, 24047, 26874, 26936, 51500, 26560,
         21456, 54224, 39369,  3456, 18885, 27583, 52650, 51628, 51496, 26593,
         53312, 35174, 47398, 47870, 47721, 63785, 64249, 29367, 47238, 47140,
         56833, 43566, 37206,  7158, 39166,  6699,  3234, 18612, 51500, 51342,
         51502, 10680, 15392, 43646, 43701, 48446, 62284,  8668, 37367, 22776,
         20834, 41804, 39294, 35944, 59826, 20562, 22475, 53569,  8047,  1481,
          3259, 25512, 13496, 23234, 14563, 35191, 39967, 52514, 54564, 53877,
         40309, 47295,  6630,  3720, 24076, 33093, 39280, 55802, 52394, 51236,
         52588, 35216, 13333, 38044, 19916, 52990, 26298,  7658, 11306, 51468,
         27128, 34217, 41573, 48053, 58392, 63545, 47363, 47164, 55592, 56022,
         63991, 55733, 65239, 56565, 48245, 44351, 47396, 41694, 43124,  6582,
          3132, 52718,  6372,  7915, 53538, 45386, 22883,  3616, 11896, 23243,
          7350, 52411,  2480, 19784, 18856, 51628, 51496, 51436, 53220, 11898,
         39543, 45686, 15036, 42529, 28184, 14501, 34918, 39348, 63734, 55587,
         23498, 34760, 36331, 22466,  6374,  9889, 18351, 48687, 41190, 14462,
         11824, 15896, 14435, 22098,  2556, 36025,  1824, 28602, 21729, 23791,
          7287, 56467, 30314, 28866, 55475,  3249, 59505, 12451, 37537, 55487,
          7665, 23243, 23654, 19638, 18638, 34683, 52668, 51336, 51640, 59576,
         27580, 52711, 53246, 60472, 27048, 10728, 39780, 43510, 64220, 47481,
         64219,  2149, 39137, 56497, 15086,  2391, 22498, 15972, 43566,  2101,
         23185, 26368, 40488, 41254, 47358, 64702, 51180,  5115,  4041, 52449,
         18088, 58253, 30763,  2118, 23903, 26750, 37626, 47142, 22646, 47206,
          6258,  3578, 39651,  7228, 56760, 47138,  6335, 36377, 26392,  7320,
         26368, 19592, 51208, 43434, 18938, 19938, 40811,  3512, 18618, 51500,
         43408, 34025,  8807, 31323, 43703, 64230, 41828, 14430,  7852, 31236,
         41782, 39208, 45608, 43132, 27738, 54248, 56288, 55540, 40293, 45760,
          2174, 55934, 21039, 38341, 40265, 22706,  6263, 56323, 13034, 39117,
          3310,  8129, 24414, 20442, 52708, 35096, 63087, 41109, 39191, 39474,
          6340, 56546, 52744,  4259, 39624, 23807, 19654, 26782, 17164, 62653,
         43983, 14577, 64949, 31899, 56762, 51644, 52188, 45783, 47142,  6815,
         23934, 22743, 39637, 39163, 11442, 19893, 18732, 26800, 44640, 41860,
         43828, 30760,  6373, 23915,  3296, 28556, 10469, 40371, 26750, 28172,
         13848, 37615, 42354, 18423, 36280, 59744, 20706,  6837, 38953, 40287,
         40679, 52562, 26668, 18584, 51626, 51518, 51628, 19902, 18876, 51240,
         10744, 20082, 52970, 36650, 27566, 52715, 60704, 51484, 19372, 46120,
         41334, 20805, 35175, 55657, 41855, 47393, 47286, 62453, 47595, 31443,
         63922, 47350, 47822, 47976, 55666, 36145, 34728, 33524, 47838, 43718,
          2597, 46356, 36760, 15932,  2244, 56012, 55489, 12910, 32887,   518,
         31920, 53955, 39136, 22187,  9488,  5760,  1033, 26008, 62909, 43079,
         14939, 47348,  6388, 39152,  5289,  1297,  5800, 25868, 39344, 43262,
         15084, 56955, 28236, 21961, 21833, 21441, 32462, 17676, 20408,  3880,
         27581, 47714, 47654, 56374, 52496, 51256, 28092, 51500, 26664, 34625,
          4553,  8129, 18837, 51641, 18878, 27134, 60414, 52730, 28586, 19962,
         52524, 51472, 42345,  4275, 22009,  8517, 20823, 31585, 47327, 39190,
         45694, 33653,  6764, 46898, 14432, 32871, 47734, 39221,  2853, 14636,
         61216, 23585, 41766, 56841, 47920, 22619, 59726, 47220,  8136, 36728,
         24271, 23794,  3770, 51492, 26686, 19086, 51820, 19644, 59818, 51596,
         18600, 59644, 27068, 18734, 52666, 59582, 18878, 51372, 19900, 18472,
         59692, 43451, 12971, 10791,   614,  2678, 32288, 33381,   599, 55927,
         35364, 10806, 14911, 11007,  6372, 30368,  8534, 14971, 10733,  7586,
         57132, 35415, 10367, 23028, 39603,  6304, 14703, 14825,  8420, 39156,
          3313, 11936, 28556, 38998, 47730, 39222, 65384, 39493,  6853,  7208,
         55010, 35501, 24126, 23803, 40181, 18466, 19900, 43512, 53146, 51966,
          3424, 52024, 59624, 52652, 51630, 59696, 59368, 30310,  9197, 14519,
          8421, 13289, 14931, 10534,  6259, 60712, 18710, 40164,  2790, 15076,
         13868,  8767, 10879,  7912, 14534, 30962, 15087, 11966, 56481, 39590,
         39094, 11881, 11914, 39155, 55466]], device='cuda:0')
```
</details>
<details>
<summary>Show Tokens for Sample 2</summary>

```text
tensor([[43009, 43331,  7931, 19943, 45179, 13161, 24475, 13143, 28993, 32593,
         12049, 61577, 41094, 63620, 57082, 41175, 41885, 23032, 17803, 43486,
         37701, 40193, 45728, 64126, 41518, 39477, 39444, 46220, 41310,  4567,
         17403,  1858,  7391, 50065, 41637, 47663,  9791, 41901, 40324, 13373,
         47369, 65125, 23993, 47405, 13247,  4765, 61167, 51947, 35827, 30021,
         29539, 31353,  4917, 45881, 62331, 10153, 30465, 15228, 23833, 63647,
         63111, 65159, 45779,  4590, 45525, 48003, 34489, 46625, 43949, 48035,
         39566, 56714, 63004,  2628, 23586,  7521, 43076, 39700, 36347, 21040,
         10925, 31390, 49207, 24571, 39238, 37479, 23331, 17427, 53133, 45927,
         62918, 13251, 62118, 23154,  2871,  1320,  8125,  2855, 20011, 37171,
           102, 15150, 48362, 65337, 57149, 10138, 16315, 28559, 51151, 33750,
         61911, 33279,  1223, 45545, 13163, 55475, 62347, 48907, 62443, 39869,
         22969, 31641,  7048, 32021, 64651, 47758, 45582, 48042, 64496, 15995,
         47594, 41292,  9937, 20733, 45527, 39339, 47766, 56999, 43991, 29547,
         24391, 22359, 62951, 47758, 22583,   551, 11246, 22488, 23435, 23960,
         22682,   686, 39174, 64725, 42793, 46076, 20806, 37669, 58412, 55386,
         12583, 12750, 55993, 50925, 18267,  4903, 23840, 16391, 40292,  6502,
          2662, 15210, 58909,  4539,  8548, 12646, 32186, 31330, 18189, 36728,
         10606, 42808,   886,    70, 57274, 52203, 27390, 17723, 34745, 17851,
         49578, 44155, 37224, 33239, 43967,  1704, 20529,  7429, 15379, 62083,
         62087, 47805,  5644, 13113, 14777, 15805, 53918, 41670, 50603, 62914,
         62708, 44020,  6774, 31512, 23720, 55822, 47798, 63224, 33781, 55987,
         45993, 24355, 45487,  6406,  4563,  2026, 60361, 56955, 56636,  3512,
         28139, 36577, 14789, 47255, 42297, 43149, 29317, 56105, 22456, 43455,
         16315, 46051, 54919, 43694, 43638, 40860, 62909, 47586, 41134, 50838,
         32639, 55524, 64190, 41334, 37668, 37680, 36931, 33381,  2018, 34745,
         56565, 51685, 43749, 43374, 54586, 50828, 45730, 63695, 64764,  6510,
         40316, 49010, 33367, 47974,  8548, 24520, 17278,  2416, 59245, 56888,
         56637, 44410, 40803, 51494, 19290, 49919, 17145, 20107, 38783, 56888,
         40254, 50728, 12801, 15891, 31243, 45353, 62331, 20936,  8511, 15191,
         44985, 29217, 23139, 45835, 65267, 55740, 39848, 41078, 35174, 33928,
         19361, 43366, 61667, 62149, 43110, 34745, 55224, 39262, 45924, 53762,
          6691, 10367,  6463, 25756, 47544, 33309,  3637, 49973, 27261, 43512,
         39400, 37844, 13271, 64507, 12957,  3752, 19435, 45221, 61863, 33351,
           933, 21368,  8089,  4072, 19627,  2483, 38252,  8654,  7036, 37717,
         29271, 39431, 16908, 45806, 61892, 40690, 42521,  2405,  2339, 39768,
         60986, 19566, 35800, 61173, 35413, 14950,  6662, 42396, 63020, 43142,
         33898, 34723,  2919, 12591, 43374, 57272, 50022, 18879, 49356, 58073,
         39489, 47456, 47799, 50949, 45556, 61894, 65471, 21624,  8540, 54729,
         25412, 60109, 57209, 48508, 60924,  7762, 39509, 37446, 35244, 62601,
         43687, 47758,  3809, 47313, 64459, 63915, 41844, 23263, 65143, 57212,
         19899, 22426, 19331, 51915, 54372, 41175, 64427, 31347, 11125,  8058,
         41183, 12979, 48041, 63875,  6282, 63680, 53953, 37365, 55701, 40400,
         25753, 63913, 41652,   940, 56889,  7484, 20346, 22411, 17298,  2451,
         61121, 35429,  8742, 10797, 31144, 13274, 15337,  4614, 47118, 40953,
         23947, 49847, 36762, 52859, 51492, 51941, 45307, 45959, 62379, 45643,
         37777,  5676, 53178,  4431,  8654, 54201, 51695, 21835, 33574, 64382,
         42793, 64184, 37527, 22191, 21613, 37847, 43886, 53771, 49177, 45051,
         41638,  6844, 58998, 51755, 19194, 49017, 56889, 40251, 38498, 20363,
         40996, 41638, 48869,  9253, 47119, 42040, 64168, 35111, 47106, 40938,
         65435, 14565,  6555, 64939, 20217, 20381, 41647, 43662, 51138, 63080,
         39286, 39525, 14776, 31995, 15338, 18333, 45654, 41548, 47820, 51837,
         60009, 56123, 57149, 12186, 12218, 27029, 42443,   953, 13081, 45775,
         54931, 18077, 54889,  8558,  2703, 22872, 18222, 45748, 47799, 56215,
         44014, 55426,  6113, 62409, 48038, 21868, 21487, 21439,  6585, 56080,
         47496, 47760, 27391, 24546, 19663, 52895, 36858, 18815, 51600, 39235,
         39509, 41542, 55740, 28705, 43693, 33327, 21210, 19087, 17101, 51083,
         39233, 38915, 65502, 45305,   838, 14760, 31211, 23240,  2943, 39718,
         47780, 38565, 45222, 33094, 22015, 50532, 52223, 19450, 58989, 56889,
         48508, 37914,  5511, 63136, 41782, 63766, 39572, 63625, 54944,  4940,
          8573, 46047, 62374, 50333, 50699,  2855,   805, 55997, 19071, 37354,
         41734, 64262, 53799, 22532, 40303, 45228, 33607,  6944,  4617,  6684,
         50717, 52157, 35249, 50541]], device='cuda:0')
```
</details>
<details>
<summary>Show Tokens for Sample 3</summary>

```text
tensor([[44529, 43238, 46054, 37622, 39349, 55476, 47254, 63912, 44781, 33495,
         47862, 47540, 34476, 22463, 46022, 47852, 63740, 63938, 39348, 63686,
         56184, 38826, 53053, 56753, 39350, 48296, 63669, 55701, 64255, 33527,
         48102, 38836, 44730, 44985, 43671, 55662, 56062, 39268, 39284, 64356,
         65262, 35574, 39606, 47284, 56232, 44730, 38968, 47478, 64802, 56042,
         39622, 47720, 55648, 55632, 39270, 47458, 56760, 36863, 37316, 45414,
         39869, 36853, 40815, 47326, 63992, 56748, 52411, 43766, 47742, 39550,
         34102, 48946, 47342, 47734, 56170, 53233, 55416, 64340, 39266, 39030,
         55351, 55602, 47414, 47158, 55604, 56628, 55358, 37734, 62280, 39926,
         57324, 36537, 43774, 38966, 36222, 52783, 64250, 39854, 63526, 37670,
         37734, 37732, 39716, 38964, 55606, 55607, 22581,  6182, 15206, 31025,
          7477, 39550, 37735, 34174, 51179, 54130, 54118, 39204, 38682, 40617,
         39102, 46398, 38831, 44022, 62442, 56186, 52750, 56059, 46046, 37732,
         55668, 55662, 47430, 39252, 39220, 56372, 56368, 35934, 56572, 47820,
         64486, 55786, 56808, 63860, 39188, 63866, 34658, 36863, 37885, 23547,
          3571]], device='cuda:0')
```
</details>

## Reconstructed Audio
Using the tokens, we can reconstruct the original audio for each sample. Here are the reconstructed audios.

Reconstructed Audio Sample 1:

<audio controls>
<source src="audio/speaker_generated.wav" type="audio/wav">
Your browser does not support the audio element.
</audio>

Reconstructed Audio Sample 2:

<audio controls>
<source src="audio/nana_1_generated.wav" type="audio/wav">
Your browser does not support the audio element.
</audio>

Reconstructed Audio Sample 3:

<audio controls>
<source src="audio/speaker_female_generated.wav" type="audio/wav">
Your browser does not support the audio element.
</audio>

This concludes the demo of our audio tokenization and reconstruction process. The ability to tokenize and reconstruct audio accurately has significant implications for various applications in audio processing and machine learning.