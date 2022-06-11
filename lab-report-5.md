# LAB REPORT 5

---

For this lab report, I have decided to use our group's representative markdown-parser repository (belongs to Nuojinli Xu). 

[Link to her repository](https://github.com/NuojinliXu/markdown-parser)

[Link to the lab 9 repository](https://github.com/nidhidhamnani/markdown-parser.git)


---

## Vim Diff comparison

I used ```vimdiff``` to display the difference in results between the cse15lsp22 markdown parser and the one from our group's markdown parser.
```
vimdiff my-markdown-parser/results.txt cse15lsp22-markdown-parser/results.txt
```

![](https://user-images.githubusercontent.com/103203293/173171547-0939c5f7-96e8-4f6f-a90a-aabc9b45c971.png)

As shown in this screenshot, there were some test files that produced different results for both our group's implementation of markdown-parser and the markdown-parser provided for lab 9.
For this lab report, I will focus on test files [194](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/194.md) and [201](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/201.md).


---

## First test file (194)

![](https://user-images.githubusercontent.com/103203293/173172181-57e9d97e-3d56-4892-904b-678f98579cd1.png)

- **Our result:**

![](https://user-images.githubusercontent.com/103203293/173172923-a46df7a3-11f7-4a45-89c4-e581bd1f0962.png)

- **Lab result:**

![](https://user-images.githubusercontent.com/103203293/173172971-9685a53b-a87b-48c5-8d9a-265b802cfe28.png)

Since "url" isn't actually a link, the expected output should just be ```[]```, so our group's implementation was correct. Looking at the lab's markdown parser, it seems that the problem was in this chunk of code that checks for opening and closing brackets and parenthesis. Our code seems to detect whether there's something between the closing bracket and the opening parenthesis, whereas the lab's code doesn't seem to do that and goes straight to finding the index of the open parenthesis. 
![](https://user-images.githubusercontent.com/103203293/173176816-1c6f0168-56c4-41ff-a103-62e68cafcdda.png)


---

## Second test file (201)

![](https://user-images.githubusercontent.com/103203293/173172221-7627b437-8ba6-4dad-b3f5-671bbc13782c.png)

- **Our result:** 

![](https://user-images.githubusercontent.com/103203293/173173044-686a019b-b36a-4117-9f27-d3573bc8bd99.png)

- **Lab result:**

![](https://user-images.githubusercontent.com/103203293/173173007-76a61bcd-9783-4d63-8519-6a295e32c042.png)

Since "baz" isn't a link, the expected output should just be ```[]```, so our group's implementation was correct. Looking at the lab's markdown parser, it seems that the problem is the same as the previous test file in that the code doesn't take into consideration that there could be something between the closing bracket and the opening parenthesis.
![](https://user-images.githubusercontent.com/103203293/173176816-1c6f0168-56c4-41ff-a103-62e68cafcdda.png)


---
