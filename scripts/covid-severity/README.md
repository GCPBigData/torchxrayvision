Data is here: [Pneumonia severity scores for 94 images](https://github.com/ieee8023/covid-chestxray-dataset/blob/master/annotations/covid-severity-scores.csv)

  - **geographic_extent_mean**: The extent of lung involvement by ground glass opacity or consolidation for each lung. The total extent score ranged from 0 to 8.		
  - **opacity_mean**: The degree of opacity. The total opacity score ranged from 0 to 6.

License: CC BY-SA Creative Commons Attribution-ShareAlike

These are from the follow paper:
Cohen, Joseph Paul, et al. Predicting COVID-19 Pneumonia Severity on Chest X-Ray with Deep Learning. May 2020, http://arxiv.org/abs/2005.11856.

```
@article{Cohen2020Severity,
title = {Predicting COVID-19 Pneumonia Severity on Chest X-ray with Deep Learning},
author = {Cohen, Joseph Paul and Dao, Lan and Morrison, Paul and Roth, Karsten and Bengio, Yoshua and Shen, Beiyi and Abbasi, Almas and Hoshmand-Kochi, Mahsa and Ghassemi, Marzyeh and Li, Haifang and Duong, Tim Q},
url = {http://arxiv.org/abs/2005.11856},
year = {2020}
}
```

To run the CLI:

```
$ python predict_severity.py 2966893D-5DDF-4B68-9E2B-4979D5956C8E.jpeg
geographic_extent (0-8): 5.978744940174467
opacity (0-6): 4.169582852893416

# or to output a saliency map:
$ python predict_severity.py 01E392EE-69F9-4E33-BFCE-E5C968654078.jpeg  -saliency_path heatmap.jpg

```

