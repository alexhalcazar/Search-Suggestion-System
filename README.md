# Search Suggestions System

## Problem Description
You are given an array of strings products and a string searchWord.  
Design a system that suggests at most three product names from products after each character of searchWord is typed.  
Suggested products should have common prefix with searchWord.  
If there are more than three products with a common prefix return the three lexicographically minimums products.  
Return a list of lists of the suggested products after each character of searchWord is typed.  

**Example 1**

Input:
```js
const products = ["mobile", "mouse", "moneypot", "monitor", "mousepad"];
const searchWord = "mouse";

const suggestedProducts = searchSuggestions(products, searchWord);
console.log(suggestedProducts);

//Output: [["mobile","moneypot","monitor"],["mobile","moneypot","monitor"],["mouse","mousepad"],["mouse","mousepad"],["mouse","mousepad"]]
```

**Example 2**

Input:
```js
const products = ["havana"];
const searchWord = "havana";

const suggestedProducts = searchSuggestions(products, searchWord);
console.log(suggestedProducts);

//Output: [["mobile","moneypot","monitor"],["mobile","moneypot","monitor"],["mouse","mousepad"],["mouse","mousepad"],["mouse","mousepad"]]
```
**Constraints:**

1 <= products.length <= 1000  
1 <= products[i].length <= 3000  
1 <= sum(products[i].length) <= 2 * 104  
All the strings of products are unique.  
products[i] consists of lowercase English letters.  
1 <= searchWord.length <= 1000  
searchWord consists of lowercase English letters.  
