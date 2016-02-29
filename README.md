=====================================
1. Bigram with Laplace (add-one) smoothing
============================================

Training set perplexity:      3761.0670
Test set perplexity:          5026.4188
Test set (no OOV) perplexity:          4240.7228
Jumbled sentences: True answer perplexity: 4240.7228

====================================
2. Bigram with Lidstone (add-lambda) smoothing, lambda = 0.001
==========================================
Training set perplexity:      130.2321
Test set perplexity:          1127.9460
Test set (no OOV) perplexity:          747.5098
Jumbled sentences: True answer perplexity: 747.5098


============================
3. Trigram with Lidstone (add lambda) smoothing, lambda = 0.001
===================================
Training set perplexity:      57.0905
Test set perplexity:          6657.3808
Test set (no OOV) perplexity: 			4896.8260
Jumbled sentences: True answer perplexity: 4896.8260

============================================
4. Trigram with interpolation and backoff estimator 
Listone(add-lambda) smoothing, lambda = 0.001
interpolation, with uniLambda = 0.6, biLambda = 0.3, triLambda = 0.1
==============================================
Training set perplexity:      61.8521
Test set perplexity:          685.1490
Test set (no OOV) perplexity:          520.4729
Jumbled sentences: True answer perplexity: 520.4729


=====================
5. Quadragram with interpolation and backoff estimator
lambdaQuadra = 0.6, lambdaTriple = 0.2, lambdaBinary = 0.1, lambdaUni = 0.1
=========================================
Training set perplexity:      172.4509
Test set  perplexity:          1146.6610
Jumbled sentences: True answer perplexity: 940.5801


=====================
6. Bigram with Kneser-Ney Smoothing
=================================
Training set perplexity:      334.3562
Test set (no OOV) perplexity:          364.3267
Test set  perplexity:          ?
Jumbled sentences: True answer perplexity: 364.3267

------------------------------
So far the best model is Bigram with Kneser-Ney smoothing, which give a constant around 350 perplexity. However, the test set perplexity (with OOV) is shown as a question mark, for which the reason is unclear to me. -