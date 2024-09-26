# TASK 1

Create a directory named `project` and:
```bash
mkdir project
```

- enter the directory and create three empty text files: `file1`, `file2`, `file3`
```bash
touch file1
touch file2
touch file3
```
- open each file one by one using the text editor (Vim or Nano), enter some text, and save it to the file
```bash
vim file1
vim file2
vim file3
```
- display the contents of each file with the `cat` command
```bash
cat file1
cat file2
cat file3
```

# TASK 2

Display the sorted content of the user's home directory (Windows: C:\Users[username], Linux: /home/[username].
```bash
ls -l /c/Users/[username]
```

# TASK 3

Display the content of any directory, recursively. Also, show the files details and sizes in mega-bytes.
```bash
ls -R .venv/
```

# TASK 4

Create the following directory tree:

├── America
│   ├── Canada
│   ├── Mexico
│   ├── USA
│   │   ├── Chicago
│   │   ├── Dallas
│   │   ├── Miami

```bash
mkdir America
mkdir America/Canada
mkdir America/Mexico
mkdir America/USA
mkdir America/USA/Chicago
mkdir America/USA/Dallas
mkdir America/USA/Miami
```

## TASK 4.1

Display recursively the content of the America directory to validate hierarchy.
```bash
ls -R America/
```

## TASK 4.2

Go to the Canada directory, and from within this folder, inside the Dallas directory create a new text file called KFC (ie. America\USA\Dallas\KFC.txt)
```bash
cd America/Canada/
touch ../USA/Dallas/KFC.txt
```

## TASK 4.3

From within the Canada directory, create an Acapulco directory inside the Mexico directory.
```bash
mkdir ../Mexico/Acapulco
```

## TASK 4.4

From within the Canada directory, print out the content of the USA directory.
```bash
ls ../USA/
```

## TASK 4.5

From within the Canada directory, pass the root directory list to the tortilla.txt file (redirection to operator >). This file is to be located in the Mexico folder.
```bash
ls /c/ > ../Mexico/tortilla.txt
```

## TASK 4.6

Display the last line of the tortilla.txt.
```bash
tail -1 ../Mexico/tortilla.txt
```

## TASK 4.7

From within the Canada directory, copy the tortilla.txt file to the Dallas directory.
```bash
cp ../Mexico/tortilla.txt ../USA/Dallas/
```

## TASK 4.8

Move to the Dallas directory, and rename the tortilla.txt file to nachos.txt.
```bash
cd ../USA/Dallas/
mv tortilla.txt nachos.txt
```

## TASK 4.9

Delete the Mexico directory with all its contents.
```bash
rm -r ../../Mexico/
```
