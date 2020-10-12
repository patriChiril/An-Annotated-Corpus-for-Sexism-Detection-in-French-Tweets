# An Annotated Corpus for Sexism Detection in French Tweets
This repository contains the first French corpus annotated for sexism detection composed of about 12,000 tweets (see [corpus_SexistContent.csv](https://github.com/patriChiril/An-Annotated-Corpus-for-Sexism-Detection-in-French-Tweets/blob/master/corpus_SexistContent.csv)) according to a novel characterization of sexist content-force relation inspired by speech acts theory and discourse studies in gender. We distinguish different types of sexist content depending on the impact
on the addressee: **sexist hate speech directly addressed to a target**, **sexist descriptive assertions** not addressed to the target, or **reported assertions** that relate a story of sexism experienced by a woman.

Sexism is often expressed by using gender stereotypes. In order to force the classifier to learn from generalized concepts rather than words which may be rare in the corpus, we adopt several replacement combinations consisting in replacing some words/expressions that trigger sexist content by their generalized term ([stereotype_list.txt](https://github.com/patriChiril/An-Annotated-Corpus-for-Sexism-Detection-in-French-Tweets/blob/master/stereotype_list.txt) contains a manually built lists of words often used in sexist language).



# Citing & Authors
If you find this repository helpful, feel free to cite our publication [An Annotated Corpus for Sexism Detection in French Tweets:](https://www.aclweb.org/anthology/2020.lrec-1.175/)

```
@inproceedings{chiril2020annotated,
  title={An Annotated Corpus for Sexism Detection in French Tweets},
  author={Chiril, Patricia and Moriceau, V{\'e}ronique and Benamara, Farah and Mari, Alda and Origgi, Gloria and Coulomb-Gully, Marl{\`e}ne},
  booktitle={Proceedings of The 12th Language Resources and Evaluation Conference},
  pages={1397--1403},
  year={2020}
}
```

If you use our manually built stereotype word list, feel free to cite our publication [He said “who’s gonna take care of your children when you are at ACL?”: Reported Sexist Acts are Not Sexist:](https://www.aclweb.org/anthology/2020.acl-main.373/)

```
@inproceedings{chiril2020he,
  title={He said “who’s gonna take care of your children when you are at ACL?”: Reported Sexist Acts are Not Sexist},
  author={Chiril, Patricia and Moriceau, V{\'e}ronique and Benamara, Farah and Mari, Alda and Origgi, Gloria and Coulomb-Gully, Marl{\`e}ne},
  booktitle={Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics},
  pages={4055--4066},
  year={2020}
}
```



