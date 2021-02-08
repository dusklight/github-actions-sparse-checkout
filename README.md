# github-actions-sparse-checkout

This repo contains a GitHub Action that demonstrates sparse checkout.

![Sparse Checkout Demo](https://github.com/dusklight/github-actions-sparse-checkout/workflows/Sparse%20Checkout%20Demo/badge.svg?branch=main)

Refer to this [blog post](https://blog.dusklight.com/2021/01/github-actions-sparse-checkout.html) for more information.

View the action file: [.github/workflows/sparse-checkout-demo.yml](https://github.com/dusklight/github-actions-demo/blob/main/.github/workflows/sparse-checkout-demo.yml)

This repo has the following structure and files.  The [sparse checkout action](https://github.com/dusklight/github-actions-demo/runs/1798956420?check_suite_focus=true#step:10:5) will only checkout `blue-folder/project1/**` folder.

```
📂 blue-folder             ┓
 ├─📂 project1             ┣━ Only this folder will be checked out
 │  ├─📄 largeFile10MB.bin ┃
 │  └─📄 textFile1.txt     ┛
 ├─📂 project2
 │  ├─📄 largeFile7MB.bin
 │  └─📄 textFile2.txt
📂 red-folder
 ├─📂 project3
 │  └─📄 textFile3.txt
 └─📂 project4
    └─📄 textFile4.txt
```
