# What is this ?

    konsoleLog is a simple utility function that helps you debug your JS code in a better way.

# Installation

    `npm install konsoleLog --save`


# Example 1

```

    import konsoleLog from 'konsoleLog'

    var API_data = {
        name: 'Hrishikesh',
        github: 'sskywalker'
    };
    
    //normal logging

    console.log(`Api data1 : ${API_data}`); 
        //Api data1 : [object Object]

    //with konsoleLog

    konsoleLog `Api data1 : ${API_data}`
        //Api data1 : {name: 'hrishikesh' , github: 'sskywalker'}


```

# Example 2

```

    import konsoleLog from 'konsoleLog'

    try{
        nothing();
    }
    catch(err){
        konsoleLog `Error : ${err}`; 
         // Error : ReferenceError : nothing is not defined at <Your error stack>
    }

```
    