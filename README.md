# Important :-

### Flutter :-

	Project Structure :-
		
		1) .idea :-
				Stored Project Related Settings.
		
		2) Android :-
				android plateform specific resources , settings & codes.
				 Used when we require android related changes.
			   
		3) Build :-
				testing mode - code created in executable file.
				used for dibugging purpose when we run app.
				we can find all relising related files like apk.
			   
		4)  IOS :-
				plateform specific resources , settings & codes.
				IOS/platform related changes can be made here.
				runnable runnerXWorks file stored here.
		   
		5)  Lib :-
			   Library folder
			   all dart/flutter related filed are inside this folder.
			   maximum useing folder / main folder.
			   entry point for a flutter app.( main.dart file )
			   
		6) test :-
			   used to improve user expriende or test user experience.
			   test folder contains any test related folders that you want to test.
			   if we decide to write test/tests cases, we will be adding code here.
			   
		7) .gitignore :-
				   vcs ( version control system )
				   removes unNessery files.
				   push, pop, pull etc opractions can be performed.
				   files which we do not want to push are putted here.
				   
		8) .metadata :-
			   conteins data related to data.
			   all flutter related settings and data are managed here.
		   
		9) .packages :-
			   2 types of packages :-
				   inbuild packages - predefined packages or packages which is defined by flutter.
				   user define packages - user createdpackages.
				
				The .package file holds the path to each of the libraries/packages in our local computer.
			   
		10) pubspec.yaml file :-
				contains flutter app specific metadata and configurations 
				configuration dependencies such as external packages, image assets, font files ,app version etc.
				you can make changes in pubspec.yaml file to add external dependcies. 
				
		11) pubspec.lock file :-
			    dependent on pubspec.yaml file.
			    creats log files
			    helper file created next to the pubspec.yaml file.
			    it lists the specific versions of each dependency that package use in app and ensures the version stays consistant across different developes matchine.
		    
		12) README.md :-
					used when we create GIT repository.
					used to contain information about project and how to use project or specification of projrct/feature.

---
### Dart :-

---
	-> Focus On Front end user interface.
	-> Object  Oriented + Strongly typed(at compile time type of variable bust be known.)
	-> It is Combination Of java , javascript and c#.
	-> Developed BY Google In 2011.
	-> Extremly Fast development cycles and fast execution and startup times.
	-> Use of async and wait for asychronous prigramming.
	-> Dart is one of very few language that is well suited to being compiled both AOT ( Ahed of time ) and JIT ( Just in time ). 
	
	Note :-
		JIT - Reloads only 1 page 
		AOT - Develops Whole app is ready it is compiled in AOT and combines it  in single .dart file.
		dart file is stored under lib( Library ) Folder.

	print() :-
		To print something in console.
	
	stdin :-
		stdin.readLineSync(); - to read user input line from console in string formate.
	
	stdout :-
		stdout.write() - for write something in console.
		,$ is used for printing value of variable
			Ex:-
				stdout.write('Your name is ,$name');

	Class & Object :-
		Same As Java
		No need to use "new" keyword when inicialising object in new versions.
		Ex :-
			class demo{}
			
					demo(); // For Creating Object.

	Datatypes :-
		 numbers - 0 to 9
		 double - flotting point vslues
		 bigint - large integer number
		 character - for alfanumeric data
		 string - arrar of characters
		 boolean( conditional ) - true or false
			 Ex :- 
				 bool a = true;
		 collection ( List And Hash map ) - store multiple values in single variable

	Declaraction of variables :- 
		
		=> By Default value of every variable is null.
		Syntax :- 
			datatype variable_name;
		
		Ex :- 
			int a;            // A Variable which can not be nullable
			int? a;           // A Variable which can be nullable

	Use of var & dynamic variable declaraction :-

	var :-
		var subject = "Maths" // Automatically set the type string but type can not change further.

	Dynamic declaraction :-

		-> can change type of variable when overwride.
		var building;             // By Default dynamic datatype which means value/dataType can change further.
		
		building = "d";    // string
		building = 3;      // int

Function in Dart :-
	function is block code which can be use for data reusability.
	
	Syntax :-
		return_type function_name(){ 
			// function body
		}
	
	Ex :-
		void printName(){             //Function declaraction
			print("Your name");         // Function Defination
		}
	
	List in Dart :-
		used to store multiple data values.
		Similar to array.
		
		array - datatype must be same of all elements
		list = datatype may be different of different elements.
	
	List Functions :-
		add() :- to add value at last in list
		addAll(list) :- To add all value at last from other list
		insert(index,value) :- To add data at perticular index
		insertAll(index,list) :- To add all value from index from other list
		to update list value index is use [2] = "value" will update value at 2nd index.
		replaceRance(start,end,[list]) :- to replace value between start to end.
		removeLast() :- to remove value from last in list.
		remove(data) :- to remove data value from list.
		removeAt(index) :- To remove data at index.
		removeRange(start,end) :- to remove value between start to end.
		
		length :- To get length of list.
		reverse :- to reverse the list.
		first :- to get first element.
		last :- to get last element.
		isEmpty :- to check element empty or not.
		isNotEmpty :- to check element not empty or not.
		elementAt(index) :- to get element present at index.
		
	Maps in dart :-
		Used to store value in key-value pair.
		Maps are very flexible and can mutate their size based on the requirenements.
		key must be unique 
		No restriction on type of data that goes in a map datatype.
		
		Syntax :-
			var variable_name = { key1:value , key2:value2,...};
	
		Ex :- 
			var map_name = {
				'key1' : 'hello',
				'key2' : 10
			}
		
		To print map :-
			map_variable_name to print whole map
			map_variable_name[key] to print value of key from map if key in not found then returns null.
			
# Flutter

## Widget in Flutter :-

	In flutter all widget classes are awailable.

### Text Widget :-

	-> The text widget displays a string of text with single style.
	-> The string might break across multiple lines or might all be displayed on the same line depending on the layout consstraints.
	-> For multiple styling in flutter there is TextSpanning (Richtext widget) is used Like fontsize,fontfamily etc styles. 
	
	Ex :- 
		body: Center(  
			child: Container(  
			height: 200,  
			width: 200,  
			color: Colors.blue,  
				hild: Center(  
				   child: Text(  
				     'Hello welcome to my app',  
				     style: TextStyle(  
				         fontSize: 25,  
				         color:Colors.white,  
				         fontWeight: FontWeight.bold  // or FontWeight.w800 or others for custom.  
				   ),    
				)  
			),  
			 
	
### Button widget :-
	-> Buttorns are the graphical control elements that provids
	-> A user to trigger an event such as taking actions, macking choices, searching things and many more. They can be placed anywhere in our UI like dialogs, forms, cards, toolbars, etc.
	-> Types of buttons :-
		 1. Text button (Flat button).
		 2. Elevated button (Raised button).
		 3. Outlined Button

	Ex :-
		child: TextButton( //TextButton or ElevatedButton or OutlinedButton  
			child: Text('Button 1',),
				onPressed: () {
					print('The Button is clicked.');  
				  },
			),
	
### Adding an Image :-

	To add an image we require directory of images generaly named assets>images.
	To add anything from out of the project we required to update pubspec.yaml file which will sytnchronise with project.
	
	in pubspec.yaml file we need to uncomment assects to use the images
	to de that
	 Go to project>pubspec.yaml inside the yaml file uncomment
		assets:
		   - assets/images/

		Note :-
			indentation is must to use assets
			the - will be just under the 3rd position like under the second s from assets.

	Ex :-
		child: Image.asset('assets/images/vvp logo.png'),
