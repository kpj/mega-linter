<!-- markdownlint-disable MD003 MD020 MD033 MD041 -->
<!-- @generated by .automation/build.py, please do not update manually -->
<!-- Instead, update descriptor file at https://github.com/megalinter/megalinter/tree/main/megalinter/descriptors/java.yml -->
# JAVA

## Linters

| Linter                           | Configuration key          |
|----------------------------------|----------------------------|
| [checkstyle](java_checkstyle.md) | [JAVA](java_checkstyle.md) |

## Linted files

- File extensions:
  - `.java`

## Configuration in MegaLinter

| Variable                  | Description                   | Default value |
|---------------------------|-------------------------------|---------------|
| JAVA_FILTER_REGEX_INCLUDE | Custom regex including filter |               |
| JAVA_FILTER_REGEX_EXCLUDE | Custom regex excluding filter |               |


## Behind the scenes

### Installation

- Dockerfile commands :
```dockerfile
ENV JAVA_HOME=/usr/lib/jvm/java-1.8-openjdk
ENV PATH="$JAVA_HOME/bin:${PATH}"
```

- APK packages (Linux):
  - [openjdk8](https://pkgs.alpinelinux.org/packages?branch=edge&name=openjdk8)
