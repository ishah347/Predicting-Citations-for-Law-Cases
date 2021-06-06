# Predicting-Citations-for-Law-Cases

We use LEGAL-BERT models (BERT transformer pre-trained on a large legal corpus) to predict cases that any particular case cites to in a specific state (North Carolina). First, we perform topic modeling on processed case text using Latent dirichlet allocation (LDA) to reduce the overall size of models and narrow the focus. Within 14 idenified topics, 11 of them are determined to be the primary topic for any one case. We fine-tune a different LEGAL-BERT model (11 in total) with multiclassification head specific for that topic cluster.
