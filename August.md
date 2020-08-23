[Collatz Conjecture](https://edabit.com/challenge/KRoiyj53QPfvubpPk)
```javascript
function collatz(n) {
	let arr = [n];
	while(n!=1){
		if(n%2 === 0){
			n=n/2;
		}else{
			n=(n*3)+1;
		}
		arr.push(n);
	}
	return [arr.length, Math.max(...arr)];
}
```

[Clear the Fog](https://edabit.com/challenge/cHNEFGeQrH3nonwJw)
```javascript
function clearFog(str) {
	return /[fog]/gi.test(str)===true?str.match(/[^fog]/gi).join(''):"It's a clear day!";
}
```

[Count Letters in a Word Search](https://edabit.com/challenge/6QNPoEjY8DLGKPiqr)
```javascript
function letterCounter(arr, letter) {
	return arr.flat(Infinity).filter(x=>x==letter).length;
}
```

[How Many Solutions Does This Quadratic Have?](https://edabit.com/challenge/x2DEtfqm4RhGcziw9)
```javascript
function solutions(a, b, c) {
	return (b * b - 4 * a * c)>0?2:(b * b - 4 * a * c)==0?1:0;
}
```

[Neutralisation](https://edabit.com/challenge/HzxTqSHLmRC3zEfXb)
```javascript
function neutralise(s1, s2) {
	return [...s1].map((x,i)=>x==[...s2][i]?x:0).join('');
}
```

[Simulate the Game "Rock, Paper, Scissors"](https://edabit.com/challenge/2n6kGrNsqpexmvJhQ)
```javascript
function rps(s1, s2) {
	return s1==s2?"TIE":s1=="rock"&&s2=="scissors"||s1=="paper"&&s2=="rock"||s1=="scissors"&&s2=="paper"?"Player 1 wins":"Player 2 wins"
}
```

[Recursion: String Palindromes](https://edabit.com/challenge/K595YtSroZHAAzvhW)
```javascript
function isPalindrome(str) {
		if (str.length < 2) {
        return true;
    }
    if (str[0] == str[str.length - 1]) {
        return isPalindrome(str.substring(1, str.length - 1));
    }
    return false;
}
```

[Quarantine TP](https://edabit.com/challenge/xhrEw5w9N45TfsgiY)
```javascript
function tpChecker(home) {
	let res = Math.floor((home.tp*500) / (57*home.people));
	return res>14?`Your TP will last ${res} days, no need to panic!`:`Your TP will only last ${res} days, buy more!`;
}
```

[Check if the String is a Palindrome](https://edabit.com/challenge/2kyS2ESQqPaoZhNSd)
```javascript
function isPalindrome(str) {
	str = str.replace(/[&\/\\#, +()$~%.'":*?<>{}\-!]/g, '').toLowerCase();
	return  [...str].reverse().join('') == str;
}
```
[What is 100% in CSS?](https://wattenberger.com/blog/)

[Reformatting the Date](https://edabit.com/challenge/CJo2NPyHDb5YyDu2S)
```javascript
function convertDate(date) {
	let datum = new Date(date);
	return [datum.getMonth()+1, datum.getDate(), datum.getFullYear()];
}
```

[Split Item Codes](https://edabit.com/challenge/Trog78Qz4bGNLFh6M)
```javascript
function splitCode(item) {
	return [item.split(/[0-9]/)[0], +([...item].filter(x=>Number.isInteger(+x)).join(""))];
}
```

[25-Mile Marathon](https://edabit.com/challenge/DvwY43tNMdEpW4kKu)
```javascript
function marathonDistance(d){
	return d.map(x=>Math.abs(x)).reduce((s,x)=>s+=x,0)==25;
}
```

[Remove Surrounding Duplicate Items](https://edabit.com/challenge/cW5gZqYEv6bszrNSw)
```javascript
function uniqueInOrder(sequence) {
	return [...sequence].filter((x,i)=>i!=0||i!=sequence.length-1?x!=sequence[i+1]:'');
}
```

[Remove Repeated Letters](https://edabit.com/challenge/cgSmKhr3Hzez2Pt9n)
```javascript
function unrepeated(str) {
	return [...new Set([...str])].join('');
}
```

[The Museum of Incredibly DULL Things](https://edabit.com/challenge/9ukwiKyv8R9NHSt3d)
```javascript
function removeSmallest(arr) {
	let index = arr.indexOf(Math.min(...arr));
	arr.splice(index, 1);
	return arr.length?arr:[];
}
```

[Check if a String is a Mathematical Expression](https://edabit.com/challenge/YREKdhk9gK5HByM7r)
```javascript
function mathExpr(expr) {
	return [...expr].filter(Number).length==2?true:false;
}
```

[Abbreviating a Sentence](https://edabit.com/challenge/ktqDpdPrFApaQpcCi)
```javascript
function abbreviate(sentence, n) {
	n = n?n:4;
	return sentence.split(" ").filter(x=>x.length>=n).map(x=>x[0].toUpperCase()).join("");
}
```

[Calculate the Shortest Distance Between Two Points](https://edabit.com/challenge/W6H4Bcaiu6svso7vT)
```javascript
function shortestDistance(str) {
	let arr = str.split(",");
	return +Math.sqrt((arr[2] - arr[0])**2 + (arr[3]-arr[1])**2).toFixed(2);
}
```

[Sum of all Evens in a Matrix](https://edabit.com/challenge/yiMSg6cNNCeJDQo3b)
```javascript
function sumOfEvens(arr) {
	return arr.flat(Infinity).reduce((s,x)=>x%2==0?s+x:s,0);
}
```

[Distance Between Two Points](https://edabit.com/challenge/caeSeQ3K53GMQKenX)
```javascript
function getDistance(a, b) {
	return +Math.sqrt((b.x - a.x)**2 + (b.y - a.y)**2).toFixed(3);
}
```

[Compound Interest](https://edabit.com/challenge/2GmmGPrktkTzTthdB)
```javascript
function compoundInterest(p, t, r, n) {
	return +(p* Math.pow((1 + (r/(n))), (n*t))).toFixed(2);
}
```

[Count the Towers](https://edabit.com/challenge/LcEFe7PsxTqciY62v)
```javascript
function countTowers(towers) {
	return Math.max(...towers.map(x=>x.map(y=>y.replace(/[ ]/g,"").length/2)).flat(1));
}
``````

[Malthusian Catastrophe](https://edabit.com/challenge/4BeTkEwBXeuSKJTYe)
```javascript
function malthusian(foodGrowth, popMult) {
	var population = 100;
	var food = 100;
	var year = 0;
	do{
		food += foodGrowth;
		population *= popMult;
		year++;
	}while(food>population)
	return year;
}
```

[The Million Dollar Fence](https://edabit.com/challenge/kKcEHvyJemCPKkjPZ)
```javascript
function constructFence(price) {
	return new Array(1000000/(+price.split("$")[1].replace(/,/g,''))).fill('H').join('');
}
```

[Valid Hex Code](https://edabit.com/challenge/cWvYKp8JTE9ozC6NF)
```javascript
function isValidHexCode(str) {
	return /^#([0-9A-F]){6}$/i.test(str);
}
```

[Capitalize the Last Letter](https://edabit.com/challenge/WrXmsGDGxqkjNCZtw)
```javascript
function capLast(txt) {
	return txt.split(" ").map(x=>x.slice(0, x.length - 1) + x[x.length-1].toUpperCase()).join(" ");
}
```

[Is One Array a Subset of Another?](https://edabit.com/challenge/3ymGugubc4gTfcqcR)
```javascript
function isSubset(arr1, arr2) {
	return arr1.every(x=>arr2.indexOf(x)!==-1);
}
```

[Return the Index of All Capital Letters](https://edabit.com/challenge/cRAqXCgyYnjdgktEq)
```javascript
function indexOfCaps(str) {
	return [...str].map((x,i)=>i).filter((y)=>[...str][y] === [...str][y].toUpperCase() && /^[A-za-z]*$/.test([...str][y]));
}
```

[Functioninator 8000](https://edabit.com/challenge/xpGPz3QCAhtsZrWeW)
```javascript
function inatorInator(inv) {
	return /[^AEIOU]$/i.test(inv)?inv+'inator '+inv.length+'000':inv+'-inator '+inv.length+'000';
}
```

[Rectangle in Circle](https://edabit.com/challenge/Qqo3rXrDEQ6kc4PqR)
```javascript
function rectangleInCircle(w, h, radius) {
	return Math.sqrt(w**2 + h**2) < 2*radius;
}
```

[First N Vowels](https://edabit.com/challenge/2FBEMqxiZ2z9efgQB)
```javascript
function firstNVowels(s, n) {
	let arr = [...s].filter(x=>x.match(/[AEIOU]/i));
	return n<=arr.length?arr.slice(0,n).join(""):"invalid";
}
```

[Returning an "Add" Function](https://edabit.com/challenge/xtv5ZT7xDsHyrshTq)
```javascript
function add(n) {
	return function(m){
		return m+n;
	}
}
```

[ES6: Destructuring Objects VI](https://edabit.com/challenge/7yCojzi2ye2Fn6iQT)
```javascript
const str = `
function shirtSize({size = "big"}={}) { 
  return size;
}
`
```

[RegEx: Character Classes XII ⁠- \t](https://edabit.com/challenge/w2abzEMHE7SFLQzDq)
```javascript
const REGEXP = /\t /g
```

[Syncopated Rhythm](https://edabit.com/challenge/9JGd2TFCb33SQ2rhL)
```javascript
function hasSyncopation(s) {
	var fil = s.split("#").filter(x=>x!='' && x!= '.');
	return /.#/g.test(s)?fil.length==0?true:fil.filter(x=>x.length%2==0).length>0:false
}
```

[Compounding Letters](https://edabit.com/challenge/aThG46eyi9LhGdTFY)
```javascript
function accum(str) {
	return [...str].map((x,i)=>x.toUpperCase() + x.repeat(i).toLowerCase()).join("-");
}
```

[ES6: Destructuring Objects X](https://edabit.com/challenge/sWzEwh5cXaAY7yEoo)
```javascript
let names = []

let users = [
  { name: "John", email: "john@example.com" },
  { name: "Jason", email: "jason@example.com" },
  { name: "Jeremy", email: "jeremy@example.com" },
  { name: "Jacob", email: "jacob@example.com" }
] 

const str = `
	for(let {name} of users) {
			names.push(name)
	}`
```

[ES6: Destructuring Arrays V](https://edabit.com/challenge/gMXdPQQbMdws8fTxC)
```javascript
const str = `[,protocol,host,path] = parsedURL`
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
``````

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
```
