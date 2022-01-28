# Menu-project

This is a javascript practice projectby John Smigla.

HTML and CSS written by John Smigla. 

I added the JavaScript functionality 

## Concept Learnt

1. The reduce method to get the unique categories.

	```js
	    const categories = menu.reduce(function(values, item){
	    if(!values.includes(item.category)){
	      values.push(item.category);
	    }
	    return values;
	  }, ['all'])
		```
2.	The map method used to loop through an array and display each item using the HTML structure of a single Item and the join method to turn the new array of categoryBtns to a single string.

	```js
	  const categoryBtns = categories.map(function(category){
	    return `<button type="button" 
	              class="filter-btn" 
	              data-id=${category}>
	              ${category}
	            </button>`
	  }).join('')
	  btnContainer.innerHTML = categoryBtns;
	```

BTW, John is an awesome teacher!