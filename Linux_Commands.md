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

