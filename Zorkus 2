import time
inventory = []
location = ""
sword = "sword"
coins = "coins"
pickaxe = "pickaxe"
OldSword = "OldSword"

knife = "knife"
DoorKey = "DoorKey"
LVL2Sword = "LVL2Sword"

print("------------      ")
print("------------      ")
print("       / /        ")
print("      / /         ")
print("     / /          ")
print("    / /        |--------|    -----|   |--| |--/  |-|   -|   |----    ")
print("   / /         |   __   |    |  | |   |  | | /   | |  | |   | ___\      ")
print("  / /          |  |__|  |    |  |_|   |   >^|    | |  | |   | |__      ")
print("------------   |        |    |  |     |  |>| \   | |__| |   ---| |   ")      
print("------------   |________|    |  |     |__| |__\  |______|  |___/_/    ")
print("Technologic® 2023. Game made by Arthur Keller Technologic CEO and head Programmer in 2023. Welcome to Zorkus 2! The Stealing Of The Throne! Your commands are 'use', 'south', 'west', 'north', 'up', 'down' 'grab', 'fight'.")

import time
inventory = []
location = ""
sword = "sword"
coins = "coins"
pickaxe = "pickaxe"
OldSword = "OldSword"
knife = "knife"
DoorKey = "DoorKey"
LVL2Sword == "LVL2Sword"

while True:
	print("Your inventory is:",inventory)
	print("Your location is: ",location)
	
	
	if location == "":
		print("Type 'start' to start")
	elif location == "Mirky Forest":
		print("You are in the Mirky Forest. Your possible exits are east and west.")
	elif location == "Stone Boulder":
		print("You found a stone boulder that you can't get past. If you have a pickaxe then type 'use' to use it. Your possible exits are east and north. Also the rock re-comes after you mine it so when you come back you must mine it down again as this is a curse Zorkus put on the land.")
	elif location == "Fence":
		print("You find a Fence and can't get past. Your possible exits are south.")
	elif location == "Outside The Old Cottage":
		print("You are outside an Old Cottage and it seems unlocked. Your possible exits are west and east. You can enter the cottage with 'east'.")
	elif location == "Old Cottage":
		print("You are indside the Old Cottage. Your possible exits are west and south.")
	elif location == "Chest 1":
		print("You can unlock the chest with 'grab'. Your possible exits are north.")	
	elif location == "Open chest 1":
		print("Your possible exits are north.")
	elif location == "Old Mine":
		print("Wow! You are inside a Old Mine. This is what the rock was blocking! Your possible exits are north and east.")
	elif location == "Abandoned Village":
		print("You find an abandoned Village. It looks like hell here, as the houses are broken and there are tons of dead bodies everywhere. Your possible exits are south, west, south, east, and north.")
	elif location == "Abandoned Village Street":
		print("You find a dead end! Your possible exits are south.")
	elif location == "Ambush 1":
		print("You find a Zombie Soldier! You can see that he is blocking a path out of the Village, and he had a knife! You can attack him with 'fight'. Your possible exits are east.")
	elif location == "Woods":
		print("You find yourself in the Woods of the cursed skeletons! Your possible exits are east, south, north, west. ")
	elif location == "Smithy Workshop":
		print("If you have a knife and a OldSword, then type 'use' to make a LVL 2 sword! Your possible exits are west.")
	elif location == "Colossal door":
		print("If you have the key to this door, type 'use' to use it. Your possible exits are east.")
	elif location == "Ambush 2":
		print("You find an Ogre! Type 'fight' to fight him. Your possible exits are north.")
	elif location == "Chest 2":
		print("Type 'grab' to open the chest. Your possible exits are south.")
	elif location == "Open chest 2":
		print("Your possible exits are south.")
	elif location == "Tower Entrance":
		print("You make it to Zorkus's Tower! Type 'use' to open the doors. Your possible exits are east.")
	elif location == "Throne Room":
		print("You are now inside Zorkus's throne room! You see him on the throne, and suddenly the doors shut! Your exits are blocked! Type 'fight' to fight Zorkus.")
	
	enter = input(": ")
	
	if location == "":
		if enter == "start":
			print("After claiming your throne and banishing the evil emperor Zorkus, you restored peace to the forgotten land. But 1 year later, Zorkus came back with an army of ogres, and took your throne. You are now the man who must reclaim the throne, and restore peace once again...")
			time.sleep(10)
			location = "Mirky Forest"
	elif location == "Mirky Forest":
		if enter == "east":
			print("You find an old cottage.")
			location = "Outside The Old Cottage"
		elif enter == "west":
			print("You find a stone boulder you can't get past.")
			location = "Stone Boulder"
	elif location == "Stone Boulder":
		if enter == "east":
			location = "Mirky Forest"
		elif enter == "use":
			if pickaxe in inventory:
				print("You get past the stone boulder!")
				location = "Old Mine"
			else:
				print("You don't have a pickaxe")
		elif enter == "north":
			print("You find a fence.")
			location = "Fence"
	elif location == "Fence":
		if enter == "south":
			location = "Stone Boulder"
	elif location == "Outside The Old Cottage":
		if enter == "east":
			print("You went inside the Old Cottage.")
			location = "Old Cottage"
		elif enter == "west":
			location = "Mirky Forest"
	elif location == "Old Cottage":
		if enter == "south":
			print("You find a chest! What a surprise!")
			location = "Chest 1"
		elif enter == "west":
			location = "Outside The Old Cottage"
	elif location == "Chest 1":
		if enter == "grab":
			if pickaxe in inventory:
				print("The chest is empty.")
			else:
				print("You get a pickaxe!")
				inventory += [pickaxe]
				location = "Open chest 1"
		elif enter == "north":
			location = "Old Cottage"
	elif location == "Open chest 1":
		if enter == "north":
			location = "Old Cottage"
	elif location == "Old Mine":
		if enter == "north":
			print("You leave the mine!")
			location = "Abandoned Village"
		elif enter == "east":
			location = "Mirky Forest"
			print("You go through the boulder (as you minded it) and to the Mirky Forest.")			
	elif location == "Abandoned Village":
		if enter == "south":
			location = "Old Mine"
		elif enter == "west":
			print("You find a zombie soldier!")
			location = "Ambush 1"
		elif enter == "north":
			location = "Abandoned Village Street"
		elif enter == "east":
			print("You find a old smith workshop!")
			location = "Smithy Workshop"
	elif location == "Abandoned Village Street":
		if enter == "south":
			if OldSword in inventory:
				location = "Abandoned Village"
			else:
				print("You find an old sword on the way back!")
				inventory += [OldSword]
				location = "Abandoned Village"
	elif location == "Ambush 1":
		if enter == "east":
			location = "Abandoned Village"
		elif enter == "fight":
			if OldSword in inventory:
				print("You kill the soldier!")
				location = "Woods"
			else:
				print("You don't have a sword and run away!")
				location = "Abandoned Village"
	elif location == "Woods":
		if enter == "west":
			print("You find a colossal locked door!")
			location = "Colossal door"
		elif enter == "east":
			print("You go back to the village.")
			location = "Abandoned Village"
		elif enter == "south":
			print("You find an Ogre!")
			location = "Ambush 2"
		elif enter == "north":
			print("You find a chest!")
			location = "Chest 2"
	elif location == "Colossal door":
		if enter == "use":
			if DoorKey in inventory:
				print("You unlock the door!")
				location = "Tower Entrance"
			else:
				print("You don't have the key and turn back.")
				location = "Woods"
		elif enter == "east":
			location = "Woods"
	elif location == "Ambush 2":
		if enter == "fight":
			if LVL2Sword in inventory:
				if DoorKey in inventory:
					print("The Ogre dies! You then go back to the woods.")
					location = "Woods"
				else:
					print("You kill the Ogre and get the DoorKey! You then go back to the woods.")
					inventory += [DoorKey]
					location = "Woods"
			else:
				print("You don't have a LVL2-Sword and turn back.")
				location = "Woods"
		elif enter == "north":
			location = "Woods"
	elif location == "Chest 2":
		if enter == "grab":
			if knife in inventory:
				print("The chest is empty.")
				location = "Open chest 2"
			else:
				print("You get a knife!")
				inventory += [knife]
				location = "Open chest 2"
		elif enter == "south":
			location = "Woods"			
	elif location == "Smithy Workshop":
		if enter == "use":
			if LVL2Sword in inventory:
				print("You already have a Lvl 2 sword.")
				location = "Smithy Workshop"
			elif (knife in inventory) and (OldSword in inventory):
				print("You craft a level 2 sword!")
				inventory += [LVL2Sword]
				location = "Smithy Workshop"
			else:
				print("You don't have a knife and OldSword")
				location = "Smithy Workshop"
		elif enter == "west":
				location = "Abandoned Village"
	elif location == "Open chest 2":
		if enter == "south":
			location = "Woods"
	elif location == "Tower Entrance":
		if enter == "use":
			print("You open the doors!")
			location = "Throne Room"
		elif enter == "east":
			print("You go past the Colossal Door into the woods.")
			location = "Woods"
	elif location == "Throne Room":
		if enter == "fight":
			print("You defeat Zorkus after a tough battle! You then chose to kill him, so he would not harm the world anymore.")
			print(" |   |  |  |\ | | | |")
			print(" |_^_|  |  | \| . . .")			  
			break
		
	
					
			          
