Arabic Punctuation Restoration (Muraqqam Challenge)
My part of a team project for the Muraqqam Challenge by Dal Challenges, in partnership with the King Salman Global Academy for Arabic Language.
Task: restore seven punctuation marks (. ، ؟ ! : ؛ -) in unpunctuated Arabic text. The metric is macro-F1, excluding the "no punctuation" class.
Approach: fine-tuned UBC-NLP/MARBERTv2 as a token classifier that predicts the punctuation after each word. The word-splitting logic is the same as in the official metric, so local validation matches the leaderboard. I held out 10% of the training data for validation.
Result: 0.640 macro-F1 on the private leaderboard (the official baseline was about 0.36).
Setup: Kaggle free-tier GPU, open-source models only, no external data.
Note: the competition data isn't included. You can get it from the competition page on Kaggle.
