---
title: 0005 - Python Scripts
---

In case you haven't figure it out yet, I'm an IBDP student and as it turns out, having a graphing calculator is a must. Mainly due to the complexity of the maths that we do. I thought that I'd go with the IB recommended one, the TI-Nspire but that one's $235 which is a bit too expensive for just two years. What about the TI-84?

The TI-84 was what I was going to go with, but I found out that the Casio CG50 has basically the exact features the TI had, at a similar price. Turns out the CG50 is just a lot faster, to the extent that I got second-hand embarrassment from watching a comparison video.

Anyway, I bought the Casio CG50 and waited for it to arrive. When it did, I quickly found out that it lives up to its reputation but one thing surprised me. You see, the calculator supports Python scripts. I'd read that it could but I didn't know what to expect. I started to tinker around within the Python app and quickly realised that I could load custom Python files onto my calculator.

Seeing the possibility to make a lot of calculations easier, I seized the opportunity. At the moment, I've just finished learning about the Binomial Theorem, a way to make expanding terms such as $(5x \times 12)^9$ a lot easier. This was what I decided to first program: a script that would solve the equation for me.

Like any good programmer, I quickly searched up if anyone had already made a script I could port over and they had! Except that they gave you the final value for the equation, whereas I wanted just the coefficients, meaning that I'd have to make it myself. I eventually found a way that I thought would work:

```
import math

print("Calculate the coefficients of (A + Bx)^n") # Calculates coefficients, not final value
A = int(input("A = "))
B = int(input("B = "))
n = int(input("n = "))

for r in range(n+1):
        
    C = (math.factorial(n) / (math.factorial(n-r) * math.factorial(r))) * (A**(n-r)) * (B**r)

    print("x power " + str(r))
    print(C)
```

What this means is that Python loads up the math library (a collection of premade scripts that I can use, so I don't have to code anything myself) and then asks me for the values of A, B, and n. Then it loops until it's calculated and outputted the coefficients for each term. Easy right? No.

You see, the part with the factorials didn't work. It would only work for the first two terms of the expansion before increasing exponentially. I searched around for a solution and found a dedicated function to find combinations, so the line looked like this: `C = math.comb(n, r) * (A**(n-r)) * (B**r)`. Excited, I hooked up my calculator to my laptop and copied the file over and tested it out.

It. Didn't. Work. Turn out, my calculator couldn't find the `math.comb()` function, meaning that I had to program it from scratch.

I then decided to make a function to calculate the factorial for any given number and then use that for each of the terms but I ran into some problems with getting the function to work properly so I decided to redesign.

There's three factorial that have to be found `n, (n-r), r` meaning that I could just make one of them work and copy it but with different variables. In the end, I came up with this solution:

```
 for i in range(1, n+1):
        factn = factn * i
		
 for i in range(1, (n-r)+1):
        factnr = factnr * i
		
 for i in range(1, r+1):
        factr = factr * i
```

With this code, I tested it out a few times, but I got the same problem as I originally had: the factorials wouldn't work. I kept tweaking the code and eventually decided to try changing the loop type as a last resort and ended up with this:

```
 while(counter <= n):
        factn = factn * counter
        counter += 1

    while(counter <= (n-r)):
        factnr = factnr * counter
        counter += 1

    while(counter <= r):
        factr = factr * counter
        counter += 1
```

For some reason this works?? I have no idea why, maybe the for loops were just bugging out, but I'm not complaining ¯\\\_(ツ)\_/¯. Now for the final test - can the calculator run it? Aaaaaand, it works!

So after a few hours of tinkering and learning how the hell you're meant to use Python, I got a functioning script. I doubt that this will be the last script I write, so I made a [GitHub repository](https://github.com/manassadasivuni/calculator-scripts) where you can download the files for yourself and use them. Just as a word of warning, the script are designed _specifically_ for the Casio CG50 so it might not work on another calculator but I'm pretty sure that the code is simple enough all devices will be able to understand it. This is because it doesn't make use of any fancier (and hence high-level) Python mechanics and uses pure logic, albeit less efficiently.

This isn't my first foray into Python. My first attempt was when I was 12 or 13 and I was following a book on how to use it but eventually lost interest. The same thing happened a few weeks ago and failed for the same reason. One of my programming friends recommended that I just pick a project and learn the language as I go and that's what I'm doing. I've found that it's a much more enjoyable way to learn as I'm not learning useless information just for the sake of knowing and learning what I need when I need it. It's like the difference between studying a textbook and finding a useful bit of information when you need it.

If you have any tips or trick on how to use Python or ideas for scripts, please send them to me; it's fun to make them and it helps me get better at my programming.