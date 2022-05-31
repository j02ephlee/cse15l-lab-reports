# LAB REPORT 4

[My markdown implementation](https://github.com/j02ephlee/markdown-parser)

[Our group markdown repository](https://github.com/NuojinliXu/markdown-parser)

[Reviewed group's markdown repository](https://github.com/NLChung9/markdown-parser)

---

## Test 1

```
`[a link`](url.com)

[another link](`google.com)`

[`cod[e`](google.com)

[`code]`](ucsd.edu)
```
How I turned it into test:
![](https://user-images.githubusercontent.com/103203293/171099842-0d16d21e-61ff-4179-b727-4b165c848538.png)

My Test (FAILED): 
![](https://user-images.githubusercontent.com/103203293/171098851-0aa8843a-9d73-4575-9836-aa7b493697bf.png)

---

## Test 2

```
[a [nested link](a.com)](b.com)

[a nested parenthesized url](a.com(()))

[some escaped \[ brackets \]](example.com)
```
How I turned it into test:
![](https://user-images.githubusercontent.com/103203293/171099694-27cf24da-69fc-4254-b19a-2d262d53ab78.png)

My Test (FAILED):
![](https://user-images.githubusercontent.com/103203293/171099253-308f1512-6dea-48fb-94fe-cc341fa7a2f0.png)

---

## Test 3 

```
[this title text is really long and takes up more than 
one line

and has some line breaks](
    https://www.twitter.com
)

[this title text is really long and takes up more than 
one line](
https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule
)


[this link doesn't have a closing parenthesis](github.com

And there's still some more text after that.

[this link doesn't have a closing parenthesis for a while](https://cse.ucsd.edu/



)

And then there's more text
```
How I turned it into test:
![](https://user-images.githubusercontent.com/103203293/171100173-f687e620-c86e-49aa-9e7f-d4540e6de3d6.png)

My Test (FAILED):
![](https://user-images.githubusercontent.com/103203293/171099336-28c36047-12f6-4d4c-978d-cd01bc426039.png)

---

# The Other Group's Code and Tests

_NOTE: minor changes were made since the original code and test files do not contain the code snippets for this lab_

Changes to their code to make it work with the snippets for this lab report:
![](https://user-images.githubusercontent.com/103203293/171103152-80989cdb-8f99-4e54-85d1-2c1e704872c2.png)


## Test 1

![](https://user-images.githubusercontent.com/103203293/171102750-7a195963-03cb-4bf7-92fa-f0e89fa6d740.png)


## Test 2

![](https://user-images.githubusercontent.com/103203293/171102819-db3b7edf-c383-43ab-9c49-6fe96722aada.png)


## Test 3

![](https://user-images.githubusercontent.com/103203293/171102897-100c8e13-5861-4aeb-bf14-d3a08bcc899d.png)


---

# QUESTION
