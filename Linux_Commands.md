# Grep

Search in File

```grep "hello" lib/abc.js```

Search in Directory

```grep "hello" lib/**/*.js```

Highlight search in color

```grep --color "hello" lib/abc.js```

Highlight search in color and show line number

```grep --color -n "hello" lib/abc.js```

Show 2 lines up and down => Context from searched text

```grep --color -n -C 2 "hello" lib/abc.js```

Search with regex

```grep --color -n -e "hello[ab]world" lib/abc.js```

# Curl

GET

```curl <URL>```

Show Header

```curl -i <URL>```

Handle Redirect

```curl -iL <URL>```

Sending Header

```curl -H "content-type:text/plain" <URL>```

Posting data

```curl -X POST -H ".." -d '{"name": "hello"}' <URL>```

Multi-line command

```
curl -X POST \
-H ".." \
-d '{"name": "hello"}' \
<URL>
```

Output to file

```curl -iL <URL> -o <FILE_PATH>```

# Find

Case-insensitive

```find . -iname *.jpg```

Find Directory

```find . -type d -name *data*```

Delete file as it finds

```find . -name "data*.js" -delete```

# Bash Script and Command Line Arguments

Arguments passed to script.sh can be get as $1, $2

```echo $1 world```

Access script.sh from anywhere

1. export PATH=$PATH:<PATH_TO_SCRIPT.SH> => Use below
2. ```chmod u+x <PATH_TO_SCRIPT.SH>```
   ```cp <PATH_TO_SCRIPT.SH> /usr/local/bin```
   
Get list of environment variables

```$env```

## Functions

Define and call

```
greet() {
  echo "hello"
}

greet
```

Pass arguments

```
greet() {
  echo "$1 hello"
}

greet "world"
```

Call method and store to a variable

```
greet() {
  echo "$1 hello"
}

greetings=$(greet "world")
echo $greetings
```

Conditional Statements

```
if [[ $USER='root' ]]; then
  echo 'root'
elif [[ $USER='home' ]]; then
  echo 'home'
else
  echo 'guest'
fi

```

   

