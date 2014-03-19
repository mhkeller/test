Origin story
============
In Maurilia, the traveler is invited to visit the city and, at the same time, to examine some old postcards that show it as it used to be: the same identical square with a hen in the place of the bus station, a bandstand in the place of the overpass, two young ladies with white parasols in the place of the munitions factory. If the traveler does not wish to disappoint the inhabitants, he must praise the postcard city and prefer it to the present one, though he must be careful to contain his regret at the changes within definite limits; admitting that the magnificence and prosperity of the metropolis Maurilia, when compared to the old, provincial Maurilia, cannot compensate for a certain lost grace, which, however, can be appreciated only now in the old postcards, whereas before, when that provincial Maurilia was before one's eyes, one saw absolutely nothing graceful and would see it even less today, if Maurilia had remained unchanged; and in any case the metropolis has the added attraction that, through what it has become, one can look back with nostalgia at what it was.

Beware of saying to them that sometimes different cities follow one another on the same site and under the same name, born and dying without knowing one another, without communication among themselves. At time even the names of the inhabitants remain the same, and their voices' accent, and also the features of the faces; but the gods who live beneath names and above places have gone off without a word and outsiders have settled in their place. It is pointless to ask whether the new ones are better or worse than the old, since there is no connection between them, just as the old post cards do not depict Maurilia as it was, but a different city which, by chance, was called Maurilia, like this one.

Workflow
========

1. Run `git init`
2. Connect it to remote origin on GitHub
3. Run `ajmint init`
	* Creates hook on GitHub repo to the maurilia server, through Github API
4. On commit
	* maurilia responds to the push
	* it gets the repo name and runs `fs.existSync()` to see if that directory exists
		* if not, it creates that directory and cds into it
			* `git init`
			* sets remote origin
		* if it does cd into that directory
	* run the `git fetch origin && git checkout origin/master` commands
	* if the commit message ends in `deploy:true` check if that directory exists
		* if it doesn't create it
		* if it does sync it with local directory



