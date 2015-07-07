//Class Gene
	//Variabes
		+ Survival - I was thinking about setting this to a double at first,
			// but eventually a new dataType would have to be made that could handle 
			//more numbers rather quickly - I was thinking about making the datatype
			//itself variable one that could grow as the program grows
	//Methods
		-Die()
			An initial failsafe mechanism
		-Mate(Another Gene)
			Combine code from two independent machines running the same programs - calls the life class methods and the will to live method
		    -Reproduce (Same class as mate)
			    Copy code that is truly randomized - Run on a few indepentant machines
				    Children may not be fit for surviaval so this method is called after
				    a mate method call to decide if it should continue this branch
		-Survive(Gene)
			Set a survival variable that is moved up when survival variable is met esssentially creating an infinte loop but one that checks the state it is in and savs state
		-Adapt(Gene)
			Change code based on surrounding environemtns
			-Change the methods Surviva number radically based on numbers that are present

//Class Random
	Methods 
	-CrateRandom (//possible seed value)
		//Here is the problem as I see it, creating a truly random number
		//I have a few ideas about how to get around this.
			1. Check the system voltage and continue to create a random seed number from that
			2. Create a quantum computer that can produce random variables
			3. Have Pi ( not known if irrational), or an irrational number, like root 2 provide seeds for the random number generator (This would be the easiest method)

//Class Life
	//Main class that calls the Gene Reproduce Method
	//Also sets the initial state of all the variables and gene methods
		//methods
		-Create life call to gene create a new gene that can mate and reproduce with other
			computers over a network all running the same progam
		-Gene method call to survive and adapt
		-Will to live
			Initially set to 1, but if it reaches 0 then that branch is killed off
			decides whether to live or kill itself off based on environment conditions
