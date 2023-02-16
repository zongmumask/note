## objdump
#### print section headers
objdump -h a.o 
#### print assembly code
objdump -d a.o
#### print relocation table
objdump -r a.o
#### print symbol table
objdump -t a.o

## clang / gcc
#### compile to object file
gcc -c a.c
#### compile to dynamic library
gcc -fPIC -shared -o libdemo.dylib lib.c

## proxy
export ALL_PROXY=socks5://127.0.0.1:1086

otool -tv 
clang++

## cocoapods

### basic
1. pod spec create NAME
2. git tag [tagname]
3. git tag -d [tagname] (remove local tag)
4. git push --delete origin [tagname] (remove remote tag)
5. git remote add origin [git URL]
6. git push --tags
7. pod repo add [privateSpecsName] [PodSpecs Git URL]

### lint
pod lib lint --verbose (local)

pod spec lint --verbose --allow-warnings (local/remote)

### submit open source code
pod trunk push NAME.podspec

### submit private code
pod repo push [privateSpecsName] NAME.podspec --allow-warnings

## symbolicatecrash
prepare three files: symbolicatecrash, .crash, .dSYM.
1. cd /Applications/Xcode.app/Contents/SharedFrameworks/DVTFoundation.framework/Versions/A/Resources
2. export DEVELOPER_DIR="/Applications/XCode.app/Contents/Developer"  
3. ./symbolicatecrash NAME.crash NAME.app.dSYM > result.crash

## git
### pull single file from remote
git checkout origin/master -- FILENAME

### squash commits into one
git rebase --interactive [commit-hash]

### delete remote branch
git push <remote_name> --delete <branch_name>


---


- The & symbol instructs commands to run in a background process and immediately returns to the command line for additional commands.