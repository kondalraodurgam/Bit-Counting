# Bit-Counting
Write a function that takes an (unsigned) integer as input, and returns the number of bits that are equal to one in the 

binary representation of that number.  Example: The binary representation of 1234 is 10011010010, so the function should return 5 
in this case


      var countBits = function(n) {
		n = n.toString(2).replace(/0/g,'').split('')
		let  count = 0;
		for (let i = 0; i<n.length; i++){
		count+= parseInt(n[i])
		}
		return count;
	};
