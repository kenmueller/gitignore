# `.gitignore`

Create a `.gitignore` file in your root directory

## Ignoring single files

**Must specify filename and extension**

```bash
example.txt
```

## Keeping single files

```bash
!example.txt
```

## Multiple files with the same extension

```bash
*.txt
```

## Multiple files with the same name

```bash
example*
```

## Folders

```bash
examples/
```

## Files inside of folders

**You can apply the same techniques for multiple files inside the root directory**

```bash
examples/example.txt
```

## Everything inside of a folder except for some files

**When first ignoring the whole folder, you must have a star at the end.**

**The star means you are ignoring the files in the folder, while not having a star means that you are ignoring the whole folder**

```bash
examples/*
!examples/example.txt
```

## Ignoring files in every directory

**This ignores all files named example.txt in every folder. You can use the same techniques for ignoring specific names or extensions with this syntax as well.**

```bash
**/example.txt
```

## Ignoring files only in the root directory

**Must include a slash in the beginning**

```bash
/example.txt
```

## Matching many characters

**This ignores files named `Example.txt` and `example.txt`. You can match against as many characters as you like at once.**

```bash
[Ee]xample.txt
```