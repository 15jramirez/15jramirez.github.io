---
layout: post
title:      "CLI Project: Anime Search"
date:       2020-10-12 02:38:05 +0000
permalink:  cli_project_anime_search
---


Where to begin. This project was a huge hurdle to get through, but accomplishing at the very end. So, let's dive in shall we. 
**ABOUT THE PROJECT **
     It starts of by asking the user the type of anime they want to pick of their chose. From there the user gets a list of the anime they can choose from as well as three options : 1.) To see the result of searches again
		                                                                                                          2.) Search for another anime listing 
		                                                                                                          3.) To exit out of the program
	    
			When it comes to searchin the result again, all the user has to put search for it again. It will be outputing only that instances of search back.  The same goes with search it will only show that instance rather than all of the anime's instances.  The final one would be extiting out of the program where when the user will exit, it will have a goodbye message along with a japanese emoticon cause after all it is anime search finder.  
		 

**Issues **
    One of the big issues I had was my prorcasination in completint the project. It did not help that I was being overzerlous with what I wanted to do with the project given how much I had time left to.
		I do have to say BINDING.PRY such a life saver to use in my coding projects. With using the pry throught out code constantly, it helped me realize tiny mistakes I kept doing. For example in one of th methods where it calls on the list and returns the same very list the user searched it would not work and get an error. The error was due to me calling the variable @anime rather than @anime_search. The code snipt is below of how it looks: 
		    if input == "list"
				print_animes_list(Anime.find_by_anime(@anime_search))
		

**Outcomes**
       I am happy that I was able to get this far. From where I first started no way will I be ever able to code this project. I still have lots to learn and review Object Orientation. But I feel accomplished on how far I've gotten. A big lesson learned as well in this project. I need to kick procrasination's butt and do things early on. 
			 Just got to keep on coding, keep on coding, coding :)
			 



