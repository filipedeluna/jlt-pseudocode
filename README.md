# Usage

Sample file - copy and paste to a new empty Tex file.

```latex

\input{CHANGE/THIS/TO/YOUR/PATH/jlt-pseudocode}

\begin{document}		
	\begin{algorithmic}[1]
		
		% Write code here
		
	\end{algorithmic}
\end{document}

````

# Example

````
\asdinterface
	\asdrequests
	\asdstatement{request()}
	\asdend
	\asdindications
	\asdstatement{indication()}
	\asdend
\asdend

\asdupon[request()]
	\asdlinecomment{some comment}
	\asdstatement{someThing()}
\asdend

\asdupon[indication()]
	\asdtrigger{someFunction()}
\asdend

\asdif[\asdin{thing}{set})]
	\asdstatement{doStuff()}
\asdelseif[someOtherCondition()]
	\asdassign{thing}{newThing}
\asdelse
	\asdsetupptimer{newTimer(t, ``Fail'')}	
\asdend
````
