# lint-configs

## Uncrustify
### Installation
1. Install uncrustify
```
$ brew install uncrustify
$ touch ~/.uncrustify.cfg | open -e ~/.uncrustify.cfg
```
2. Paste the contents of `.uncrustify.cfg` in this repo to the file you just created

### Adding to Services
1. Open `Automator` app
2. Select `Quick Action`
3. Search for `Run Shell Script` on the search text field and drag it in
4. Set the ffg properties
- Workflow receives current: **text**, in: **XCode**
- Output replaces selected text: **Checked**
- Shell script:
```
export PATH=/usr/local/bin:$PATH
uncrustify -l oc
```




