simpleComment
=============

Simple Comment Formats - Compatible with AppleDocs


###METHODS
Method group (or method sections) - Used to group some methods: <br>
```
/** @name Method Group Name */
```
Method description - Will descrive the method <br>
```
/** Method description */    
- (void)someMethod;  
/** Method description 2 */  
- (void)someOtherMethod;
```
Method description WITH params and returns <br>
  @param paramName paramDescription <br>
  @return returnDescription
```
/** Will fry a potato
* @param potato Potato's name.
* @return Returns a friedPotato.
*/
-(FriedPotato)fryPotato:(Potato) potato;
```
Code inside comments - Used if you want to explain some code in a comment <br>
  Comments inside ` character will be taken as code block in appledocs
```
//To fry a potato, use `-(FriedPotato)fryPotato:(Potato) potato;`!!
```
Comments inside methods - If you want to explain something inside a method implementation <br>
  Will comment above the line we want to explain, using only `//` not a comment block `/**  */`: <br>
```
-(FriedPotato)fryPotato:(Potato) potato
{
  //this will help us to fry the potato
  FriedPotato fPotato = [[FriedPotato alloc] initWithPotato:potato];
  //returning the fried potato....
  return fPotato;
}
```

###PROPERTIES
Will comment properties with a comment block above the `@property` declaration (only once in `.h` if it's public or `.m` if it's private for each property).
```
/**
* This is the potato used to cook:
*/
@property Potato cookingPotato;
```

###DELEGATES
We will comment delegates the same way we comment methods (see methods section). Appledocs detects and generate delegates documentation itself.

More Info:
[appleDocs](http://web.archive.org/web/20120628101954/http://gentlebytes.com/appledoc-docs-comments/)
[Markdown language](https://daringfireball.net/projects/markdown/syntax)
