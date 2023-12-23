import time
inventory = []
location = ""
spear = "spear"
landsites = []
UnpassableMountains = "UnpassableMountains"
sword = "sword"
GoldenStone = "GoldenStone"

print("------------      ")
print("------------      ")
print("       / /        ")
print("      / /         ")
print("     / /          ")
print("    / /        |--------|    -----|   |--| |--/  |-|   -|   |----    -----\ ")
print("   / /         |   __   |    |  | |   |  | | /   | |  | |   | ___\        | ")
print("  / /          |  |__|  |    |  |_|   |   >^|    | |  | |   | |__      ---")
print("------------   |        |    |  |     |  |>| \   | |__| |   ---| |        |")      
print("------------   |________|    |  |     |__| |__\  |______|  |____/ /   ----/")
print("Game made by Arthur Keller in 2023, Main programmer Arthur Keller. Welcome to Zorkus 3! The Island! Your commands are 'use', 'south', 'west', 'north', 'up', 'down' 'grab', 'fight'. Fun game: Try and find all the Land Sites!")

inventory = []
location = ""
spear = "spear"
landsites = []
UnpassableMountains = "UnpassableMountains"
sword = "sword"
raso = "raso"
GoldenStone = "GoldenStone"


while True:
	print("Your inventory is:",inventory)
	print("Your location is: ",location)
	print("Your landsites are: ",landsites)
	
	if location == "":
		print("Type 'start' to start")
	elif location == "Beach":
		print("You are at the shore of the island. Your boat is destroyed. Your possible exits are west, south and north. ")
	elif location == "Shore":
		print("Your possible exits are north.")
	elif location == "Ambush 1":
		print("You find a thunder guard! You can attack him with 'fight'. Your possible exits are east.")
	elif location == "Outside Of Cave":
		print("You are outside a cave. Your possible exits are east, south and north.")
	elif location == "Unpassable Mountains":
		print("Your possible exits are west.")
	elif location == "Cave":
		print("You are inside the cave. Your possible exits are south and west.")
	elif location == "Box":
		print("You can look inside the box with 'grab'. Your possible exits are east.")
	elif location == "Open Box":
		print("Your possible exits are east.")
	elif location == "Outside Of Sand-Tunnel":
		print("You can enter the sand tunnel with 'down'. Your possible exits are east.")
	elif location == "Sand Tunnel":
		print("You are now inside a sand tunnel! Your exit also corrupted when you came inside! Your possible exits are north.")
	elif location == "Land Of The Island People":
		print("Your possible exits are south, north, west, east.")
	elif location == "ambush 2":
		print("If you have a sword type 'fight' to use it. Your possible exits are south and west.")
	elif location == "chest 1":
		print("You can open the chest with 'grab'. Your possible exits are east.")
	elif location == "open chest 1":
		print("Your possible exits are east.")
	elif location == "Golden Stone":
		print("Sadly, you can't pass this stone due to it's holy power. Your possible exits are west.")
	elif location == "Village Trader":
		print("If you have something valueable type 'use' to trade it. Your possible exits are east.")
	elif location == "maze corridor 1":
		print("Your possible exits are south, east and west.")
	elif location == "dead end 1":
		print("You find a dead end! Your possible exits are east.")
	elif location == "maze corridor 2":
		print("Your possible exits are west, east and south.")
	elif location == "dead end 2":
		print("Your possible exits are north.")
	elif location == "maze corridor 3":
		print("Your possible exits are north and west.")
	elif location == "maze exit":
		print("Your possible exits are south and north.")
	elif location == "Temple":
		print("You find Thronus with his thunder spear! Your exits also get electrocuted! Type 'fight' to fight Thronus.")
		
		
	
	
	enter = input(": ")
	
	if location == "":
		if enter == "start":
			print("After you have finally killed Zorkus, you set sail to an island. The island is ruled by the thunder god - Thronus. You must defeat Thronus as he is devastating the island with his thunder guards and killing villagers...")
			time.sleep(9)
			location = "Beach"
		elif enter == "hacks":
			print("Do you want to use hacks? Enter 'yes' or 'no'.")
			enter = input(": ")
			if enter == "yes":
				inventory += [sword]
				inventory += [spear]
				landsites += [UnpassableMountains]
				landsites += [GoldenStone]
				inventory += [raso]
				location = "Beach"
			else:
				print("You don't use hacks but skip prolog.")
				location = "Beach"
	elif location == "Beach":
		if enter == "south":
			print("You can't go any further as there is the sea.")
			location = "Shore"
		elif enter == "north":
			print("You find a cave!")
			location = "Outside Of Cave"
		elif enter == "west":
			print("You find a thunder guard!")
			location = "Ambush 1"	
	elif location == "Shore":
		if enter == "north":
			location = "Beach"
	elif location == "Ambush 1":
		if enter == "east":
			location = "Beach"
		elif enter == "fight":
			if spear in inventory:
				print("You kill the guard and find a sand tunnel!")
				location = "Outside Of Sand-Tunnel"
			else:
				print("You don't have a spear and turn back!")
				location = "Beach"
	elif location == "Outside Of Cave":
		if enter == "east":
			if UnpassableMountains in landsites:
				print("You find the unpassable mountains.")
				location = "Unpassable Mountains"
			else:
				print("You find the unpassable mountains.")
				landsites += [UnpassableMountains]
				location = "Unpassable Mountains"
		elif enter == "north":
			print("You enter the cave.")
			location = "Cave"
		elif enter == "south":
			location = "Beach"
	elif location == "Unpassable Mountains":
		if enter == "west":
			location = "Outside Of Cave"
	elif location == "Cave":
		if enter == "south":
			location = "Outside Of Cave"
		elif enter == "west":
			print("You find a box!")
			location = "Box"
	elif location == "Box":
		if enter == "grab":
			if spear in inventory:
				print("The box is empty!")
				location = "Open Box"
			else:
				print("You find a spear!")
				inventory += [spear]
				location = "Open Box"
		elif enter == "east":
			location = "Cave"
	elif location == "Open Box":
		if enter == "east":
			location = "Cave"
	elif location == "Outside Of Sand-Tunnel":
		if enter == "down":
			location = "Sand Tunnel"
		elif enter == "east":
			print("You go back to the beach.")
			location = "Beach"
	elif location == "Sand Tunnel":
		if enter == "north":
			print("You reach the land of the island-people! (The people Thronus is hurting)")
			location = "Land Of The Island People"
	elif location == "Land Of The Island People":
		if enter == "south":
			location = "Sand Tunnel"
		elif enter == "north":
			print("You find another thunder-guard!")
			location = "ambush 2"
		elif enter == "east":
			print("You find a stone that has gold around it!")
			if GoldenStone in landsites:
				location = "Golden Stone"
			else:
				landsites += [GoldenStone]
				location = "Golden Stone"
		elif enter == "west":
			print("You find the The Village Trader!")
			location = "Village Trader"
	elif location == "ambush 2":
		if enter == "west":
				print("You find a chest!")
				location = "chest 1"
		elif enter == "fight":
			if sword in inventory:
				print("You kill the guard and find a maze!")
				location = "maze corridor 1"
			else:
				print("You don't have a sword and when you try to run away he kills you! YOU DIE!!!!")
				location = "Beach"
	elif location == "chest 1":
		if enter == "grab":
			if raso in inventory:
				print("The chest is empty!")
				location = "open chest 1"
			else:
				print("You find something looking valuable! Hmmm....")
				inventory += [raso]
		elif enter == "east":
			location = "ambush 2"				
	elif location == "open chest 2":
		if enter == "east":
			location = "ambush 2"
	elif location == "Golden Stone":
		if enter == "west":
			location = "Land Of The Island People"
	elif location == "Village Trader":
		if enter == "use":
			if raso in inventory:
				print("You trade a raso for a sword! Because he is kind though, he lets you keep some of the raso!")
				inventory += [sword]
			else:
				print("You don't have anything valueable!")
				location = "Village Trader"
		elif enter == "east":
			location = "Land Of The Island People"
	elif location == "maze corridor 1":
		if enter == "south":
			print("You go past the dead guard and to the land of island people.")
			location = "Land Of The Island People"
		elif enter == "east":
			location = "maze corridor 2"
		elif enter == "west":
			location = "dead end 1"
	elif location == "dead end 1":
		if enter == "east":
			location = "maze corridor 1"
	elif location == "maze corridor 2":
		if enter == "west":
			location = "maze corridor 1"
		elif enter == "south":
			location = "dead end 2"
		elif enter == "east":
			location = "maze corridor 3"
	elif location == "dead end 2":
		if enter == "north":
			location = "maze corridor 2"
	elif location == "maze corridor 3":
		if enter == "west":
			location = "maze corridor 2"
		elif enter == "north":
			print("You find the maze exit!")
			location = "maze exit"
	elif location == "maze exit":
		if enter == "south":
			location = "maze corridor 3"
		elif enter == "north":
			print("You exit the maze and find the temple of Thronus! You then go inside.")
			location = "Temple"
	elif location == "Temple":
		if enter == "fight":
			if sword in inventory:
				print(" ")
				print(" O |   []  \^^^^^ ")
				print("/|/  \-/-/ \    \ ")
				print("/\    /     \   /")
				print("You defeat Thronus!")
				print("YOU WIN THE LAST GAME OF ZORKUS!!!!!!")
				print("------------      ")
				print("------------      ")
				print("       / /        ")
				print("      / /         ")
				print("     / /          ")
				print("    / /        |--------|    -----|   |--| |--/  |-|   -|   |----     ")
				print("   / /         |   __   |    |  | |   |  | | /   | |  | |   | ___\       ")
				print("  / /          |  |__|  |    |  |_|   |   >^|    | |  | |   | |__    ")
				print("------------   |        |    |  |     |  |>| \   | |__| |   ---| |        ")      
				print("------------   |________|    |  |     |__| |__\  |______|  |____/ /   ")
				print("|   |  |  |\ | | | |")
				print("|_^_|  |  | \| . . .")
				break
				
		
