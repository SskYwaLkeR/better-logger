# What is this ?

    konsolelog is a simple utility function that helps you debug your JS code in a better way.

# Installation

    `npm install konsolelog --save`


# Example 1

```

    import konsolelog from 'konsolelog'

    var API_data = {
        name: 'Hrishikesh',
        github: 'sskywalker'
    };
    
    //normal logging

    console.log(`Api data1 : ${API_data}`); 
        //Api data1 : [object Object]

    //with konsolelog

    konsolelog `Api data1 : ${API_data}`
        //Api data1 : {name: 'hrishikesh' , github: 'sskywalker'}


```

# Example 2

```

    import konsolelog from 'konsolelog'

    try{
        nothing();
    }
    catch(err){
        konsolelog `Error : ${err}`; 
         // Error : ReferenceError : nothing is not defined at <Your error stack>
    }

```
    