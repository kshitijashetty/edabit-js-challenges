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

[]()
```javascript
```

[]()
```javascript
```

[]()
```javascript
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
