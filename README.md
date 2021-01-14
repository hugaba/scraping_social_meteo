# scraping_social_meteo
projet scraping meteo et réseaux sociaux par Mickaël Rebeau, Franck Madola Benae et Hugo Algaba

Le repository contien 7 fichiers:
* reddit.py
* twitter2.py
* weather.py
* reddit_AustinFC.csv
* twitter_AustinFC.csv
* weather_AustinFC.csv
* scraping.ipynb

Les fichiers python reddit.py et twitter2.csv peuvent être lancés séparément en premier lieu.
Ils permettent de générer les fichiers csv reddit et twitter (noms d'enregistrement à changer si scraping sur une nouvelle source)
* reddit.py: Pour un scraping sur une nouvelle source: 
 * modifier 'AustinFC' dans la ligne "for post in reddit.subreddit('AustinFC').hot(limit=1000):"
 * modifier reddit_AustinFC.csv' dans la ligne "posts.to_csv('reddit_AustinFC.csv')" pour ne pas écraser le fichier existant

* twitter2.py: Pour un scraping sur une nouvelle sourcec:
 * modifier 'AustinFC' dans la ligne "Username = "AustinFC"  # filter by username"
 * modifier 'twitter_AustinFC.csv' dans la ligne "c.Output = "twitter_AustinFC.csv"  # name of the desired output"
 * relancer le programme plusieurs fois en changeant les dates pour avoir un fichier csv complet (ne rajoute que les nouvelles lignes à chaque fois)

Une fois les scraping effectués sur au moins un des sites, le programme weather.py peut être lancé.

 
