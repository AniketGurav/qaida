# Qaida
Qaida is a data set of of 18569 ligatures in [Urdu](https://en.wikipedia.org/wiki/Urdu) language synthetically 
generated in 256 different fonts. The dataset consists for 3713800 training images and 1039864 test images belonging to 
18569 ligature classes. Each ligature class in the training data images rendered using 200 unique fonts while the test 
data contains each class rendered in 56 fonts. Fonts are kept unique across training and test set making it a viable for
 a font-independent ORC system.
 
Here is an example how the data looks (each row is a different class):
![](doc/img/qaida_sprite.png)

###  Introduction to Urdu Script
Urdu is a subset of [Arabic](https://en.wikipedia.org/wiki/Arabic) language and is written in a cursive script. 
It has 39 letters and is written cursively from right to left. Letters within a word are joined to form a sub-word 
called a ligature. 

###Why we made Qaida
OCR algorithms, have received a significant improvement in performance recently, mainly due to the increase
in capabilities of artificial intelligence algorithms. However this advancement is not evenly distributed over all 
languages. Urdu is also among the languages which di not receive much attention, specially in the font independent 
perspective.
One of the main reason for is intra-class variability of the letters in Urdu; unlike English and other Latin based 
languages, letters in Urdu are not constrained to only a single shape. Their shape changes with their position within
the ligature. Number of shapes per letter vary from one to four. There are almost [18,569 valid 
ligatures](http://www.cle.org.pk/software/ling_resources/UrduLigatures.htm) in Urdu which are to be recognized as 
compared to only 52 characters (excluding numbers and punctuations) in English.

Qaida is an attempt to advance the research in font independent printed Urdu test recognition by creating a large scale 
public dataset. This dataset, to the best of out knowledge is the only large multi-font Urdu dataset. 
