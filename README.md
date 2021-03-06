# Parse Gmail Atom Feed emails

*Simple command line app that parses the Atom XML feed for Gmail emails*

## Installation

```
npm install --global parse-gmail-atom
```

## Usage

```
$ USERNAME="you@gmail.com"
$ PASSWORD="password"
$ curl -u $USERNAME:$PASSWORD --silent "https://mail.google.com/mail/feed/atom" | pgmail
```

## Output

The output has the format of emails being delimited by `***EMAIL***`.  For each email portion this is the format...

```
0:  EmailId
1:  SenderName
2:  SenderEmailAddress
3:  MessageSubject
4+: MessageBody
```

*Note: those line numbers are not included in the output, just here to reference their order*