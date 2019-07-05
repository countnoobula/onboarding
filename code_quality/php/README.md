As an attempt to improve and maintain the quality of our code, we chose to use PHPMetrics as the initial implementation to help us monitor and maintain our code quality. The two primary percentage measurements that we've focused on are Code and Style.

## What must I do?
Once https://github.com/bonlineza/.github/pull/3 is merged, in every PR that you make, please take the time to fill in the appropriate section in the PR template.

Ideally, every developer receives 30 minutes a day to use for documentation and improvement towards our codebase. This is what we should strive towards to help improve our codebase.
The PHPMetric issues with the projects will be split up into Github issues on each project and can be chosen from there.

At the beginning of every week, each developer will choose an issue depending on which project they are working on. The goal is for an issue per week to be closed. The deadline for PR's is Friday 2pm.

## Rules
Below are a list of rules, that we use in our PHPMetrics.

#### STYLE
 - Closing Tag 
 - Side Effects 
 - Git Merge Conflict
 - Byte Order Mark
 - Line Endings 
 - Function Closing Brace
 - Object Operator Indent
 - Scope Closing Brace
 - Disallow Long Array Syntax
 - Line Length 
 - Space After Cast
 - Space After Not
 - Function Call Argument Spacing
 - Character Before PHP OpeningTag
 - Backtick Operator 
 - Disallow Alternative PHP Tags
 - Disallow Short Open Tag
 - Forbidden Functions 
 - Lower Case Constant
 - Lower Case Keyword
 - Lower Case Type
 - SAPI Usage 
 - Syntax 
 - Disallow Tab Indent
 - Increment Decrement Spacing
 - Language Construct Spacing
 - Camel Caps Method Name
 - Else If Declaration
 - Switch Declaration 
 - Upper Case Constant Name
 - Namespace Spacing 
 - Require One Namespace In File
 - Unused Uses 
 - Use Does Not Start With Backslash
 - Use Spacing 
 - Spread Operator Spacing
 - Parameter Type Hint Spacing
 - Return Type Hint Spacing
 - Superfluous Whitespace 
 - Doc Comment Spacing
 - Class Instantiation 

#### CODE - Functions
 - Unused Inherited Variable Passed To Closure
 - Unused Parameter
 - Call Time Pass By Reference
 - Deprecated Functions
 - Nullable Type Declaration
 - Static Closure
 - Forbidden Functions

#### CODE - Code
- Unused Variable
- Code Analyzer 
- Switch Declaration 
- Language Construct Spacing
- Element Name Minimal Length
- Max Nesting Level
- Useless Variable 
- Eval 
- Array Indent
- Empty PHP Statement
- Empty Statement 
- For Loop Should Be While Loop
- For Loop With Test Function Call
- Jumbled Incrementer 
- Unconditional If Statement
- Useless Overriding Method
- Inline Control Structure
- Disallow Multiple Statements
- Backtick Operator 
- Discourage Goto 
- No Silenced Errors
- Unnecessary String Concat
- Short Form Type Keywords
- Disallow Implicit Array Creation
- Disallow Continue Without Integer Operand In Switch
- Disallow Yoda Comparison
- Language Construct With Parentheses
- Dead Catch 
- Unused Inherited Variable Passed To Closure
- Useless Parameter Default Value
- Use From Same Namespace
- Useless Alias 
- Require Combined Assignment Operator
- Require Only Standalone Increment And Decrement Operators
- Optimized Functions Without Unpacking
- Type Cast 
- Useless Semicolon 
- Duplicate Assignment To Variable
- Forbidden Define Global Constants
- Forbidden Private Methods 
- Forbidden Final Classes 

#### CODE - Globally
- GlobalKeyword
- ForbiddenGlobals

#### CODE - Comments
- Empty Comment
- Nullable Type For Null Default Value
- Fixme
- Todo
- Forbidden Comments
- Inline Doc Comment Declaration
- Disallow Array Type Hint Syntax
- Long Type Hints
- Null Type Hint On Last Position
- Useless Constant Type Hint
- Useless Inherit Doc Comment

#### CODE - Classes
- Forbidden Public Property
- Unnecessary Final Modifier
- Property Declaration
- Class Constant Visibility
- Disallow Late Static Binding For Constants
- Modern Class Name Reference
- Useless Late Static Binding
