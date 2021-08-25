![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)  ![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)  ![Windows 10](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
# printer 
A simple library for printing rich coloured texts on console terminal.\
Designed with Cross-platform in mind


**Targets tested :**
  * Windows 10 21H1
  * Ubuntu 20.04.1 LTS
## Usage
Inculde in your C++ program by
```Cpp
#include "printer.hpp"
```
Then call the functions as you see fit

**Example :**
```cpp
//test.cpp
#include <stdio.h>
#include "printer.hpp"
int main()
{
	
	printerClearScreen();	
	
	puts("\n\n");
	printerSlowPrint("Its too cold here...z.z..z.z.zz\n");
	printerPrintText("I need to go to my room fast\n", _text_foreground_white, _text_background_red);
	printerPrintText("Maybe a coffee will do\n", _text_foreground_red, _text_background_white);
	printerPrintText("COFFEEE...\n", _text_foreground_red, _text_background_default,_text_style_underline);
	
	puts("\n\n\n\n");
	
 return 0;
}
```
**Output :**

![image](https://user-images.githubusercontent.com/86375359/130758551-3786333d-ba19-4673-a3ea-7366baa397d4.png)

## Building

For Windows,\
I used Visual Studio

For Ubuntu,\
You will need to link the **.cpp** file during build
```py
g++ printer.cpp test.cpp -o test
```

## Credits

TutorialsPoint: https://www.tutorialspoint.com/how-to-output-colored-text-to-a-linux-terminal \
Badges : https://github.com/Ileriayo/markdown-badges

Feel free to use/edit these files as you like it.
