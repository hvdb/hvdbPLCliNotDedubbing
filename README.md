# \<cliError\>



## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.
@next ! (0.18.0.pre-15)  

Run polymer build.  

Check build/bundled/src/shell.html  

Polymer micro and mini are both in there.  
Resulting in two createElement('dom-module') (and createElement("dom-module"))  And well that causes issues...  

Uncaught DOMException: Failed to execute 'registerElement' on 'Document': Registration failed for type 'dom-module'. A type with that name is already registered.
 