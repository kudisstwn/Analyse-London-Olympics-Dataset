# Analyse-London-Olympics-Dataset

import numpy as np

# Dataset from summer Olympic London, year 2012
np_olympic_country = np.array(['GBR','China','RUS','US','KOR','JPN','GER'])
np_olympic_country_Gold = np.array([29,38,24,46,13,7,11])
np_olympic_country_Silver = np.array([17,28,25,28,8,14,11])
np_olympic_country_Bronze = np.array([19,22,32,29,7,17,14])

# find country index with maximum gold
max_gold_index = np_olympic_country_Gold.argmax()

# print country with maximum gold
print(country_with_max_gold)

# country won more than 20 gold medals, use boolean indexing technique
print(np_olympic_country[np_olympic_country_Gold>20])

# print each country name with number of gold medals
# print each country name with total number of medals
for i in range(len(np_olympic_country)):
    gold_medal = np_olympic_country_Gold[i]
    country  = np_olympic_country[i]
    total_medal = np_olympic_country_Bronze[i]+np_olympic_country_Gold[i]+np_olympic_country_Silver[i]
    print('{} => gold medal {}, Total medals {}'.format(country,gold_medal,total_medal))
