
## 7. Ignoring files. File ".gitignore".

From time to time, there are files you don't want Git to check in to GitHub.

Enter ```touch .gitignore``` to create a .gitignore file.

Чтобы файла игнорился (проверка - игнора файла ```$git status```), нужно чтобы он был удален с репозитория (удаленного).
Допустим чтобы игнорился UserInterfaceState.xcuserstate внутри xcodeproj залитого на GitHub, нужно зайти в GitHub и удалить этот файл.

С помощью .gitignore можно осуществить игнор файлов по типу configuration.plist или secrets.plist - где хранятся секретные данные, ключи, токены и тп.

```
# Xcode
#
build/
*.pbxuser
!default.pbxuser
*.mode1v3
!default.mode1v3
*.mode2v3
!default.mode2v3
*.perspectivev3
!default.perspectivev3
xcuserdata
*.xccheckout
*.moved-aside
DerivedData
*.hmap
*.ipa
*.xcuserstate

# CocoaPods
#
# We recommend against adding the Pods directory to your .gitignore. However
# you should judge for yourself, the pros and cons are mentioned at:
# http://guides.cocoapods.org/using/using-cocoapods.html#should-i-ignore-the-pods-directory-in-source-control
#
# Pods/
```


