#JSHINT

```
{

    Prohibits the use of bitwise operators such as ^ (XOR), | (OR) and others. 
    Bitwise operators are very rare in JavaScript programs and quite often & is simply a mistyped &&.
    "bitwise": true,
    
    Requires you to always put curly braces around blocks in loops and conditionals.
    "curly": true,
    
    Prohibits the use of == and != in favor of === and !==.
    "eqeqeq": true,
    
    Requires all for in loops to filter object's items.
    "forin": true,
    
    Prohibits overwriting prototypes of native objects such as Array, Date and so on.
    "freeze": true,
    
    Prohibits the use of a variable before it was defined. For hoisting usages
    "latedef": "nofunc",
    
    Prohibits the use of arguments.caller and arguments.callee
    "noarg": true,
    
    Warns about "non-breaking whitespace" characters.
    "nonbsp": true,
    
    Prohibits the use of constructor functions for side-effects
    "nonew": true,
    
    Prohibits the use of unary increment and decrement operators.
    "plusplus": false,
    
    This option prohibits the use of explicitly undeclared variables.
    "undef": true,
    
    Warns when you define and never use your variables.
    "unused": false,
    
    Requires the code to run in ECMAScript 5's strict mode.
    "strict": false,
    
    Max number of formal parameters allowed per function
    "maxparams": 10,
    
    Lets you control how nested do you want your blocks to be
    "maxdepth": 5,
    
    Set the max number of statements allowed per function
    "maxstatements": 40,
    
    Sets you control cyclomatic complexity throughout your code ?
    "maxcomplexity": 8,
   
    Suppresses warnings about missing semicolons.
    "asi": false,
    
    Suppresses warnings about the use of assignments in cases where comparisons are expected. 
    "boss": false,
    
    Suppresses warnings about the debugger statements in your code.
    "debug": false,
    
    Suppresses warnings about == null comparisons.
    "eqnull": true,
    
    Suppresses warnings about the use of eval. 
    "evil": false,
    
    Suppresses warnings about the use of expressions where normally you would expect to see 
    assignments or function calls
    "expr": false,
    
    Suppresses warnings about declaring variables inside of control structures while 
    accessing them later from the outside.
    "funcscope": false,

    Suppresses warnings about the __iterator__ property
    "iterator": false,
    
    Suppresses warnings about missing semicolons, but only when the semicolon is omitted 
    for the last statement in a one-line block
    "lastsemic": false,
    
    Suppresses warnings about functions inside of loops
    "loopfunc": false,

    Tells JSHint that your code uses Mozilla JavaScript extensions
    "moz": false,

    Suppresses warnings about invalid typeof operator values
    "notypeof": false,
    
    Suppresses warnings about the __proto__ property
    "proto": false,
    
    Suppresses warnings about the use of script-targeted URLs
    "scripturl": false,
    
    Suppresses warnings about variable shadowing
    "shadow": false,

    Suppresses warnings about "weird" constructions
    "supernew": false,
    
    Suppresses warnings about possible strict violations when the code is running in strict mode and you use this in a 
    non-constructor function
    "validthis": false,

    Option defines globals exposed by modern browsers
    "browser": true,

    "globals": {
        "angular": false,
        "$": false
    }
}
```

#JSCS
```
{
  Requires curly braces after statements.
  "requireCurlyBraces": true,
  
  Requires operators to appear before line breaks and not after.
  "requireOperatorBeforeLineBreak": true,
  
  Requires identifiers to be camelCased
  "requireCamelCaseOrUpperCaseIdentifiers": true,
  
  Requires all lines to be at most the number of characters specified
  "maximumLineLength": {
    "value": 100,
    "allExcept": ["comments", "regex"]
  },
  
  Validates indentation for switch statements and block statements
  "validateIndentation": 2,
  
  Requires all quote marks to be either the supplied value
  "validateQuoteMarks": "'",

  Disallows strings that span multiple lines without using concatenation.
  "disallowMultipleLineStrings": true,
  
  Requires lines to not contain both spaces and tabs consecutively, or spaces after tabs only for alignment if "smart"
  "disallowMixedSpacesAndTabs": true,
  
  Requires all lines to end on a non-whitespace character
  "disallowTrailingWhitespace": true,
  
  Requires sticking unary operators to the right.
  "disallowSpaceAfterPrefixUnaryOperators": true,
  
  Disallows multiple var declaration (except for-loop).
  "disallowMultipleVarDecl": false,

  Disallows sticking binary operators to the left.
  "requireSpaceBeforeBinaryOperators": [
    "=", "+=", "-=", "*=", "/=", "%=", "<<=", ">>=", ">>>=",
    "&=", "|=", "^=", "+=",

    "+", "-", "*", "/", "%", "<<", ">>", ">>>", "&",
    "|", "^", "&&", "||", "===", "==", ">=",
    "<=", "<", ">", "!=", "!=="
  ],
  
  Disallows sticking binary operators to the right.
  "requireSpaceAfterBinaryOperators": true,
  
  Requires space before and/or after ? or : in conditional expressions.
  "requireSpacesInConditionalExpression": true,
  
  Requires space(s) before block statements (for loops, control structures).
  "requireSpaceBeforeBlockStatements": true,
  
  Requires placing line feed at file end.
  "requireLineFeedAtFileEnd": true,
  
  Disallows space after opening object curly brace and before closing.
  "disallowSpacesInsideObjectBrackets": "all",
  
  Disallows space after opening array square bracket and before closing
  "disallowSpacesInsideArrayBrackets": "all",
  
  Disallows space after opening round bracket and before closing.
  "disallowSpacesInsideParentheses": true,

  Validate jsdoc comments
  "jsDoc": {
    Checks tag names are valid.
    "checkAnnotations": true,
    
    Checks all parameters are documented.
    "checkParamExistence": true,
    
    Checks param names in jsdoc and in function declaration are equal.
    "checkParamNames": true,
    
    Checks params in jsdoc contains type.
    "requireParamTypes": true,
    
    Checks for differences between the jsdoc and actual return types if both exist.
    "checkReturnTypes": true,
    
    Reports redundant params in jsdoc.
    "checkRedundantParams": true,
    
    Report statements for functions without return.
    "checkRedundantReturns": true,
    
    Reports invalid types for bunch of tags.
    "checkTypes": true,
    
    Checks a doc comment description has padding newline.
    "requireNewlineAfterDescription": true
  },

  Disallows multiple blank lines in a row.
  "disallowMultipleLineBreaks": true,
  
  Disallows commas as last token on a line in lists.
  "disallowCommaBeforeLineBreak": false,
  
  Disallows identifiers that start or end in _.
  "disallowDanglingUnderscores": true,
  
  Disallows empty blocks (except for catch blocks).
  "disallowEmptyBlocks": true,
  
  Disallows an extra comma following the final element of an array or object literal.
  "disallowTrailingComma": true,
  
  Requires commas as last token on a line in lists.
  "requireCommaBeforeLineBreak": true,
  
  Requires member expressions to use dot notation when possible
  "requireDotNotation": {
    "allExcept": [ "snake_case" ]
  },
  
  Requires parentheses around immediately invoked function expressions.
  "requireParenthesesAroundIIFE": true
}
```
