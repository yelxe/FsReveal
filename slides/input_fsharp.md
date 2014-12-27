- title : How We Became an F# Shop
- description : An introduction to F# and how it can be implemented
- author : Trevor Exley
- theme : night
- transition : default

***

# Introducing F# to a C# Shop
  
![FSharp.org](http://fsharp.org/img/logo/fsharp256.png)

#### by Trevor Exley

***

### What is F#?
  
F# is a hybrid multi-platform language that encourages a "Functional-First" approach to programming.

***

### Who Can Use It?
  
#### OS Platforms

- Windows
- Mac
- Linux

---

### Who Can Use It?
  
#### IDEs

- Visual Studio
- Xamarin
- Mono

---

### Who Can Use It?
  
#### Programming Paradigms

- Functional
- Object-Oriented 
- Imperative

***

### And What's Wrong With C#, Exactly?

***

### Simple Implementation in C# 

    [lang=cs]
	public static int Square(int i)
	{
		return i * i;
	}

	public static int SumOfSquares(int n)
	{
		int sum = 0;
		for (int i = 1; i <= n; i++)
		{
			sum += Square(i);
		}
		return sum;
	}

---

### And Now in F# 

	let square x = x * x

	let sumOfSquares n = 
		[1..n] |> List.map square |> List.sum

***

### Tuples

#### C# 
  
	[lang=cs]
	var x = new Tuple<int, string, string>(1, "John", "Smith");
  
  
Refactored as a class:  
  
  
	[lang=cs]
	var x = new MyClass(1, "John", "Smith");

---

### Tuples

#### C# 
  
	[lang=cs]
	var x = new Tuple<int, string, string>(1, "John", "Smith");
	var x = new MyClass(1, "John", "Smith");

#### F# 
  
	let x = (1, "John", "Smith")

F# cleans it up even further.

***

### What Else is Beautiful About F#?

***

### How We Got Started

***

### Build and Deployment

***

### Unit Testing

***

### Send in the Koans

***

### Conway's Game of Life

***

### Solving Business Problems

***

### Building Presentations

This presentation was created using an F# script.

***

### Resources

#### F# for fun and profit

[http://fsharpforfunandprofit.com/][1]

#### The F# Software Foundation Community Space

[github.com/fsprojects][2]  
[http://fsprojects.github.io/][3]

#### This Presentation

[https://github.com/yelxe/FsReveal][4]




[1]: http://fsharpforfunandprofit.com/
[2]: github.com/fsprojects  
[3]: http://fsprojects.github.io/
[4]: https://github.com/yelxe/FsReveal

