# Game1
A choose your own adventure game by me. 


def option(): #This is a code that lets you start the game again
    print "DO YOU WANT TO START AGAIN?  Y/N ? >>>  "
    yn = raw_input()
    if yn == "y":
        start() #start() is defined as the last block of code after def door one and def door two
    elif yn == "n":
        exit(0)	#this code ends the game

def door_one():
	print "You're at the beach! There's lots to do here. What do you want to do? \n"
	print "1. Maannnn it's so hot, I wanna get ice-cream."
	print "2. It's SO HOT and my pastey skin is burning in the sun. I wanna go get sunscreen from the car."
	print "3. Straight into the waves!"
	activity = raw_input("WHAT YOU WANNA DO? TYPE 1, 2 OR 3 >>>  ")
	if activity == "1": # you have to be really careful with these indents, check the arrows on the row numbers. They show you what's in the block.
		print "\nOK but you don't have any money, it's the day before pay day and you're broke af\n."
		print "1. I'll check the car, there's gotta be a few coins in there"
		print "2. Well luckily I'm super charming and can probably make someone buy me an icecream."
		print "3. Damn I gotta earn $3.50 RIGHT NOW\n."
		ice_cream = raw_input(">>> ")
		if ice_cream == "1":
		    print "You found a bunch of silver coins. It adds up to $3.50, the ice cream is yours!"
		    option()
		elif ice_cream == "2":
		    print "You walk up to the cool teenagers loitering outside the fish and chip shop. What do you say?\n"
		    print "1. 'Hey guys can I borrow $3.50 for a Golden Gaytime?' "
		    print "2. 'What up brothers, cool skateboards! Buy me an ice cream or you'll never see them again.' "
		    print "3. 'Hey I saw your mum and she said you had to buy me a Golden Gaytime.' "
		    teenagers = raw_input(">>> ")
		    if teenagers == "1":
		        print "'Sure' they say, and give you $3.50. Yep, you sure are charming!"
		        option()
		    elif teenagers == "2":
		        print " 'wtf is wrong with you' they say. The youngest one calls his mum and you decide to leave."
		        option()
		    elif teenagers == "3":
		        print "The youngest one calls his mum and asks her if she saw you."
		        print "Then he says 'Mum said she doesn't know who you are and she's coming to pick me up'. You decide to leave."
		        option()
		elif ice_cream == "3":
		    print "You go to the fish and chip shop and ask if you can wash dishes in exchange for $3.50."
		    print "They said you can't come behind the counter because of WHS."
		    print "You should have thought of that."
		    option()

	elif activity == "2":
		print "\nHa you don't fit in here, everyone else is so tanned and you're blinding anyone that looks at you\n."
		print "1. I don't care, they can look at me and burn their retinas off. I'm getting sunscreen"
		print "2. Oh no, you're right... Maybe I'll just get in the car and drive to another beach"
		print "3. hmm good point, I might ditch the sunscreen and try to get a tan like everyone else\n."
		sunscreen = raw_input(">>> ")
		if sunscreen == "1":
		    print "You get the sunscreen. People look at you and go blind but you don't care. You had a great time and didn't get burnt."
		    option()
		elif sunscreen == "2":
		    print "You get in the car and start driving. You try to find a quiet beach but there are people everywhere. So you just drive home for fear of causing people to go blind."
		    option()
		elif sunscreen == "3":
		    print "You lay in the hot sun, baking for an hour. That was way too long. The next day you have third degree burns. That was so dumb."
		    option()

	elif activity == "3":
		print "\nOMG THE WATER IS FREEZING WHAT THE HECK !?\n"
		print "1. I'll get used it, just keep swimming."
		print "2. Nup, I'm out. Back to the sand!"
		print "3. haha no it isn't, it's just fresh."
		water = raw_input(">>> ")
		if water == "1":
		    print "You keep swimming and your legs cramp up. You're flapping around like an idiot and the rip starts dragging you out."
		    print "A cool surfer dude comes up to you and says 'You right mate, do you want me to take you in?'\n"
		    print "1. Yes, thank you that would be great."
		    print "2. Hey dude, nah brother I'm fine out here, I swim in rips all the time."
		    surfer = raw_input(">>> ")
		    if surfer == "1":
		        print "The cool surfer dude takes you back to shore and asks you if you wanna get an ice cream sometime. You do."
		        option()
		    elif surfer == "2": 
		        print "The cool surfer dude says 'alright' but he keeps an eye on you. You start drowning and eventually you can't keep your head above water."
		        print "The cool surfer dude drags your pastey ass onto his surfboard and takes you back to shore where he performs CPR on you."
		        print "You come to and vomit sea water everwhere. The cool surfer dude is hailed as a hero and you look like a fucking idiot. Well done."
		        option()
		elif water == "2":
		    print "You haul your pastey ass back onto the sand like a beached whale"
		    option()
		elif water == "3":
		    print "A little cold never hurt anyone. You dabble in the shallows until your lips turn blue"
		    option()
		
		
def door_two():
	print "\nYou stare into the endless abyss and start seeing some weird shit. What you see??"
	print "\n1. A deeper understanding of your own mortality."
	print "2. You can literally see the wind. Like in that Disney movie but you can't remember what it's called."
	print "3. You're pretty sure you can see individual atoms in your hand if you look close enough. \n"

	insanity = raw_input("Which do you see? TYPE 1, 2 or 3: ")
	if insanity == "1":
		print "Yes, you are just a pulsing lump of flesh and you exist for no reason and have no purpose.\n"
		print "1. I like that. I like having no purpose or reason for existing, it takes the pressure off."
		print "2. This realisation takes away my fear of death entirely."
		print "3. This realisation actively makes me want to die. What's the point to life anyway."
		realisation = raw_input(">>> ")
		if realisation == "1":
			print "Yes, why should you strive to be successful when we are all going to die anyway?"
			option()
		elif realisation == "2":
			print "That's great, now you can live life with no restraints. You're welcome."
			option()
		elif realisation == "3":
			print "This realisation is legit a leading cause of suicide. Call lifeline on 13 11 14 and see if they can't talk you down."
			option()
	
	elif insanity == "2":
		print "Pocahontus. That's the movie you were thinking of."
		print "You remind your self of Pocahontus. She has super powers. Pick one:"
		print "\n1. You can learn a new language in 0.2 seconds by 'listening to your heart'."
		print "2. Your best friend is a racoon."
		print "3. Even though you're in the middle of a genocide, no one kills you because of how pretty you are. But you are abducted and taken to England...\n"
		Pocahontus = raw_input("CHOOSE 1, 2 or 3 >>> ")
		if Pocahontus == "1":
			print "Well obviously that is her best superpower...\n"
			option()
		elif Pocahontus == "2":
			print "You know the racoon has rabies right? Why would you choose that over being able to learn a new language in 0.2 seconds?!?!\n"
			option()
		elif Pocahontus == "3":
			print "That actually would be pretty useful. England sucks though.\n"
			option()

	elif insanity == "3":
		print "You can't see individual atoms lol you can see what you normally see, you're just interpreting it differently.\n"
		print "1. ...... I swear to God I can see like the electron clouds and everything."
		print "2. Oh lol yeah This abyss is crazy huh."
		print "3. I'm not even seeing with my eyes right now, I'm seeing with like, my minds eye."
		atoms = raw_input(">>> ")
		if atoms == "1":
			print "OK whatever lol"
			option()
		elif atoms == "2":
			print "Yeah SO crazy."
			option()
		elif atoms == "3":
			print "No ur not, ur seeing with ur regular eyes lol"
			option()       
			
	

			
def start():
	print "Are you ready to choose your own adventure !? Sure you are. Which door do you want to go through, door 1 or door 2?\n"		
	next = raw_input("TYPE 1 OR 2 >>>  ") #this has to be done after the code blocks
	if "1" in next:
		door_one() #if this comes before the code blocks, it won't have defined door_one() yet and you'll get an error
	elif "2" in next:
		door_two()
    
    
start() #This actually runs the start code and it is the first actual command that runs
