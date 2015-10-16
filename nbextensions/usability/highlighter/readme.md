
## The highlighter extension:

- Firstable, the extension provides <span class="mark">several toolbar buttons</span> for highlighting a selected text _within a markdown cell_. Three different \`color schemes' are provided, which can be easily customized in the stylesheet `highlighter.css`. The last button enables to remove all highlightings in the current cell. 
- This works both <span class="burk">when the cell is _rendered_ and when the cell is in edit mode</span>; 
- In both modes, it is possible to highlight formatted portions of text (In rendered mode, since the selected text loose its formatting, an heuristic is applied to find the best alignment with the actual text)
- When no text is selected, the whole cell is highlighted; 
- The extension also provides two keyboard shortcuts (Alt-G and Alt-H) which fire the highlighting of the selected text. 


![](image.gif)

## Installation:

The extension can be installed with the nice UI available on IPython-notebook-extensions website, which also allows to enable/disable the extension. 

You may also install the extension from the original repo: issue
```bash
jupyter nbextension install https://rawgit.com/jfbercher/small_nbextensions/master/highlighter.zip  --user

```
at the command line.

### Testing: 

Use a code cell with
```javascript
%%javascript
require("base/js/utils").load_extensions("usability/highlighter/highlighter")
```

### Automatic load
You may also automatically load the extension for any notebook via
```bash
jupyter nbextension enable usability/highlighter/highlighter	
```
