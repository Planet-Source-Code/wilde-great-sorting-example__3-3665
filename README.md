<div align="center">

## great sorting example


</div>

### Description

this first asks the user how many numbers they need to sort. Then, it sequentially asks the user to input those numbers. After that, it outputs all the those numbers in the right order from lowest to highest. Good example to work with arrays and looping. Sorry about the poor commenting
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[WildE](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/wilde.md)
**Level**          |Intermediate
**User Rating**    |4.3 (30 globes from 7 users)
**Compatibility**  |C\+\+ \(general\), Microsoft Visual C\+\+, Borland C\+\+, UNIX C\+\+
**Category**       |[Sorting](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/sorting__3-24.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/wilde-great-sorting-example__3-3665/archive/master.zip)

### API Declarations

```
#include <iostream.h>
#include <stdlib.h>
#include <time.h>
```


### Source Code

```
#include <iostream.h>
#include <stdlib.h>
#include <time.h>
void main(){
	int numin;
	int numbers;
	int temp[100];
	int numbers2;
	int temp2;
	cout << "How many numbers do you want to sort? ";
	cin >> numin;
	cout << "\nOk, so you want to sort " << numin << " numbers.\n Go ahead and start inputting them ";
	numbers = 1;
	for(numbers = 1; numbers < numin + 1; numbers++){
		cout << "\nEnter number " << numbers << "\n";
		cin >> temp[numbers];
		cout << "\n";
	}
	// Sorting happens here******************************************************************************
	for(numbers = 1; numbers < numin + 1; numbers++){
		for(numbers2 = numbers+1; numbers2 < numin + 1; numbers2++){
			if(temp[numbers] > temp[numbers2]){
				temp2 = temp[numbers];
				temp[numbers] = temp[numbers2];
				temp[numbers2] = temp2;
			}
		}
	}
	////sorting ends here (betweent the for loops
	for(numbers = 1; numbers < numin + 1; numbers++){
		cout << temp[numbers] << "\n";
	}
}
```

