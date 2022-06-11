# LAB REPORT 5

---

For this lab report, I have decided to use our group's representative markdown-parser repository (belongs to Nuojinli Xu). 

[Link to her repository](https://github.com/NuojinliXu/markdown-parser)

---

## Vim Diff comparison

I used ```vimdiff``` to display the difference in results between the cse15lsp22 markdown parser and the one from our group's markdown parser.
```
vimdiff my-markdown-parser/results.txt cse15lsp22-markdown-parser/results.txt
```

![](https://user-images.githubusercontent.com/103203293/173171547-0939c5f7-96e8-4f6f-a90a-aabc9b45c971.png)

As shown in this screenshot, there were some test files that produced different results for both our group's implementation of markdown-parser and the markdown-parser provided for lab 9.
For this lab report, I will focus on test files 194 and 201.

---

## First test file (194)

[Link to test file 194](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/194.md)

![](https://user-images.githubusercontent.com/103203293/173172181-57e9d97e-3d56-4892-904b-678f98579cd1.png)

- **Expected result:** []
- **Our result:** []
- **Lab result:** [url]

---

## Second test file (201)

[Link to test file 201](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/201.md)

![](https://user-images.githubusercontent.com/103203293/173172221-7627b437-8ba6-4dad-b3f5-671bbc13782c.png)

- **Expected result:** []
- **Our result:** []
- **Lab result:** [baz]

---

Since both test files didn't have an actual link, the correct output should be just a ```[]```, so for both of these test files, the results produced by the lab's markdown parser was incorrect.
