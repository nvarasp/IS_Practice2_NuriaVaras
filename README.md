# IS_Practice2_NuriaVaras
Practice 2 of interactive systems, scripting

I implemented all the features of the tutorials, and I added some more modifications: 

-By following the web instructions, there was a little error since when a sheep was dropped it was counted twice instead of once. The problem was that when sheeps collided with SheepDestroyed they increased the counter by two. Therefore, in order to solve this problem, I added an additional Boolean variable called hitByCollider which is really similar to hitByHay, since it is activated when a sheep is dropped and the condition checked at OnTriggerEnter. In this way the two counters work correctly now, and we can select the limit of dropped sheeps for the game to finish (which is set to 5 now).

-I added some background music in the game scene and title scene.

-Each time you shoot a sheep, the time between Spawns is shorter. So as the SavedSheeps counter increases, the time between each sheep is spawn is smaller, so that the difficulty of the game increases. But I set a limit, in this case time between spawns cannot be shorter than 1 second, because otherwise sheeps will be appearing from the three spawners simultaneously. 
