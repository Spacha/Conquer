# Turn-based strategy game*
* 4X: explore, expand, exploit, exterminate
* 2 or more players
* Gameplay
	* build a village
	* defend and attack
	* recuit units -> upgrade
	* 4X:
		* explore: 		at the start, the map is covered and must be explored using units
		* expand: 		build village(s), conquer enemy villages
		* exploit: 		natural resources for buildings, units, wealth
		* exterminate: 	destroy your enemies

* architecture: p2p or client-server model -> probably client-server
* Server:
	* Offers turns to the players
* Client:
	* render graphics
	* take in input
	* communicate with server
* Connection:
	* full duplex: server must be able to send messages to the client
	* websockets seems like a good idea
* Graphics:
	* pygame 2
* Data to be transmitted:
	* MOVE unit
	* ATTACK a unit
	* BUILD a building
	* UPGRADE a unit
	* SEND chat message
	* END turn