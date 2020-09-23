<div align="center">

## ^\!\!\~File Write\~\!\!^


</div>

### Description

Prompts input and writes it to a file
 
### More Info
 
File Writing


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[fritz0x00](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/fritz0x00.md)
**Level**          |Beginner
**User Rating**    |4.9 (39 globes from 8 users)
**Compatibility**  |C, C\+\+ \(general\), Microsoft Visual C\+\+, Borland C\+\+, UNIX C\+\+
**Category**       |[Coding Standards](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/coding-standards__3-32.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/fritz0x00-file-write__3-4772/archive/master.zip)

### API Declarations

```
#include <fstream.h>
#include <iostream.h>
#include <stdlib.h>
```


### Source Code

```
//by fritz300 of http://hax-studios.net
#include <fstream.h>
#include <iostream.h>
#include <stdlib.h>
int main()
{
	//** Declare Varibles, Theres only one
	char text[80];
	//** Declare pointers
	ifstream fin;
	ofstream fout;
	//** Begin; tell user what he/she is about to do
	cout << "Welcome to Fritzs Text Write program, This program (with source code included) \nwill teach you how to write text to files!\n\n";
	//** End;
	cout << "Type a word:\n";
	cin >> text;
	fout.open("c:/windows/desktop/file.txt"); //** Opens the file to write too.
	fout << "Fritzs Text Write Program Example:\n\nYou typed:\n\n\t";
	fout << text; //** Writes the input to file.txt
	fout.close();
	//** Error handler aka what happens if a error occurs
	if( !fin || !fout )
	{
		cout<<"Error has occured. Cannot open file.txt\n\n" << endl;
	}
	cout<<"\nText was successfully written to C:/windows/desktop/file.txt\n" << endl;
	cout << "\n\n\tText write program by Zak Farrington alias fritz owner of hAx Studios Ltd. <http://hax-studios.net> development team." << endl;
	system("PAUSE");
 	return 0;
}
```

