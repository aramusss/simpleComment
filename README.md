simpleComment
=============

Simple Comment Formats - Compatible with AppleDocs

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
-(friedPotato)fryPotato:(Potato) potato;
```
Code inside comments - Used if you want to explain some code in a comment <br>
  Comments inside ` character will be taken as code block in appledocs
```
//To fry a potato, use `-(friedPotato)fryPotato:(Potato) potato;`!!
```
More Info:
[appleDocs](http://web.archive.org/web/20120628101954/http://gentlebytes.com/appledoc-docs-comments/)
[Markdown language](https://daringfireball.net/projects/markdown/syntax)
