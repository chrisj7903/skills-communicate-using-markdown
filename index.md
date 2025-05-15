# This should the largest header 
stuff
## This should be smaller 2
stuff 2
### and smaller 3
#### and smaller 4
##### and smaller 5
###### smallest 6

![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)

``` cpp
void processSerialCommands() {
  if(Serial.available() > 0) {
    char readChar = Serial.read();
    if (readChar >= 42 && readChar <= 122) {                    // ignore if not between '*' and 'z' in ASCII table 
      readChar = toupper(readChar);                             // convert lower case characters to upper case
      switch(readChar){
        case 'V': if (VERBOSE)  {VERBOSE  = false; Serial << F("\nVERBOSE - off\n\n") ;}
                  else          {VERBOSE  = true;  Serial << F("\nVERBOSE - ON\n")    ;} break;
        } 
      } 
    } 
  }
```

- [x] item 1 is checked
- [ ] item 2 is not
- [ ] nor is item 3 
- [x] item 4 is checked  
