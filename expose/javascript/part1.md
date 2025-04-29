1.1 Line 9 prints "values added: 20"
1.2 Line 13 prints "final result: 20"
1.3 You should not use var because var ignores block scope meaning it can cause unexpected issues for developers because they may believe that variable should only exist within the block it was initialized but in reality it exists throughout the function.
1.4 Line 9 prints "values added: 20"
1.5 The line returns an error because result is only declared in the scope of the block and not in the scope of the function because of the use of let. Therefore, when trying to print result outside of the block it was declared in, it will say that it is not defined.
1.6 An error occurs because you cannot reassign a value to a constant varaible after it is defined to already have one.
1.7 It runs into the same issue as described in 1.6. Additionally, there would be an issue since result would only be within the scope of the block, so it would not exist in the printing line at line 13.