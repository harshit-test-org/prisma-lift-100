## Introduction

Reproduction for https://github.com/prisma/lift/issues/100

## To Reproduce

1. Clone this Repo
2. Add a 'init' migration using `prisma2 lift save --name 'init'` and `prisma2 lift up`
3. Change `posts Post` to `posts Post[]` in line number 13 of schema.prisma
4. Save another migration using `prisma2 lift save --name 'make post array'`
5. Open the README of newly created migration and view the generated SQL steps.
