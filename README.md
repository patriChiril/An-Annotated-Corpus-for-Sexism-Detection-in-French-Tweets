# An Annotated Corpus for Sexism Detection in French Tweets
This repository contains the first French corpus annotated for sexism detection (see [corpus_SexistContent.csv](https://github.com/patriChiril/An-Annotated-Corpus-for-Sexism-Detection-in-French-Tweets/blob/master/corpus_SexistContent.csv)) composed of about 12,000 tweets. [nonAnnotated.csv](https://github.com/patriChiril/An-Annotated-Corpus-for-Sexism-Detection-in-French-Tweets/blob/master/nonAnnotated.csv) contains all the collected data (the sexism corpus is a subset of it).

A tweet is annotated as **sexist** in one of the following three cases:
* the tweet contains **sexist content directly addressed to a woman or a group of women**:
```
T’es une femme je serai jamais d’accord avec toi pour du foot
(You’re a woman I’ll never agree with you about football)

les femmes qui sont en plus Dijonnaise ne parlez pas de foot sivouplai c’est comme si un aveugle manchot parler de passer le permis
(women who are also from Dijon please don’t talk about football it’s as if a one-handed blind person was thinking about getting a driving license)
```

* the tweet contains **sexist content not directed to an addressee** (the target can be a woman, a group of women, or all women, it can be named but is not the addressee):
```
Anne Hidalgo est une femme. Les femmes aiment faire le ménage. Anne Hidalgo devrait donc nettoyer elle-même les rues de Paris 
(Anne Hidalgo is a woman. Women love cleaning the house. Anne Hidalgo should clean the streets of Paris herself)

La place de la femme dans la societe moderne, est tres precise elle est dans la cuisine.
(The place of a woman in modern society is clear, it is in the kitchen.)
```

* the tweet contains a **report of an experience or a denunciation of a sexist behaviour**:
```
Mon patron m’a demandé : ”qui va cuisiner pour ton mari quand tu seras pas là ?” 
(My boss asked me: ”who’s going to cook for your husband when you’re away?”)

je m’assoupis dans le métro, je rouvre les yeux en sentant quelque chose de bizarre : la main de l’homme assis à côté de moi sur ma cuisse. #balancetonporc
(I doze in the subway, I open my eyes feeling something weird: the hand of the man sat next to me on my leg #SquealOnYourPig)
```

A tweet is annotated as **non-sexist** when the tweet has no sexist content (it may contain a specific hashtag but the content is not sexist):
```
Paris Match : journal d’investigation
(Paris Match: an investigative journal)

Laetitia Casta pas d’accord avec #balancetonporc
(Laetitia Casta disagrees with #SquealOnYourPig)
```


Sexism is often expressed by using gender stereotypes. In order to force the classifier to learn from generalized concepts rather than words which may be rare in the corpus, in [He said “who’s gonna take care of your children when you are at ACL?”: Reported Sexist Acts are Not Sexist](https://www.aclweb.org/anthology/2020.acl-main.373/) we adopt several replacement combinations consisting in replacing some words/expressions that trigger sexist content by their generalized term ([stereotype_list.txt](https://github.com/patriChiril/An-Annotated-Corpus-for-Sexism-Detection-in-French-Tweets/blob/master/stereotype_list.txt) contains a manually built lists of words often used in sexist language).



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



