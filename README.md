Origin story
============
The ancients built Valdrada on the shores of a lake, with houses all verandas one above the other, and high streets whose railed parapets look out over the water. Thus the traveler, arriving, sees two cities: one erect above the lake, and the other reflected, upside down. Nothing exists or happens in the one Valdrada that the other Valdrada does not repeat, because the city was so constructed that its every point would be reflected in its mirror, and the Valdrada down in the water contains not only all the flutings and juttings of the facades that rise above the lake, but also the rooms' interiors with ceilings and floors, the perspective of the halls, the mirrors of the wardrobes.

Valdrada's inhabitants know that each of their actions is, at once, that action and its mirror-image, which possesses the special dignity of images, and this awareness prevents them from succumbing for a single moment to chance and forgetfulness. Even when lovers twist their naked bodies, skin against skin, seeking the position that will give one the most pleasure in the other, even when murderers plunge the knife into the black veins of the neck and more clotted blood pours out the more they press the blade that slips between the tendons, it is not so much their copulating or murdering that matters as the copulating or murdering of the images, limpid and cold in the mirror.

At times the mirror increases a thing's value, at times denies it. Not everything that seems valuable above the mirror maintains its force when mirrored. The twin cities are not equal, because nothing that exists or happens in Valdrada is symmetrical: every face and gesture is answered, from the mirror, by a face and gesture inverted, point by point. The two Valdradas live for each other, their eyes interlocked; but there is no love between them.

 

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


		 deploy!!

dd

